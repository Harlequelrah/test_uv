# **`Notes uv`**
Voici mes notes sur le cours uv de openclassroom.

**url** : **https://openclassrooms.com/fr/courses/8445356-gerez-votre-environnement-python-avec-uv**

# `Commandes uv`

## `1- Intitialisation  de uv`

```cmd
uv init nom_du_projet
```

## `2- Retirer une dépendance`

```cmd
uv add dependance
```
ou pour choisir l'environnemnt active
```cmd
uv add dependance --active
```
## `3- Retirer une dépendance`

```cmd
uv remove dependance
```


##  `4- Rafraichir l'environnement virtuel si fichier pyproject.toml modifié`

```cmd
uv sync
```

## `5- Afficher un arbre des dépendances et sous-dépendances`

```cmd
uv tree
```

## `6- Créer un environnement virtuel`

```cmd
uv venv env
```

## `7- Exporter en requirements.txt`

```cmd
uv export --format requirements-txt > requirements.txt
```
ou
```cmd
uv export --format requirements-txt --no-hashes > requirements.txt
```

# `Cas récurrents`

## `1- Migration d'un projet depuis pip`

- Installation de package :

```cmd
    uv pip install -r requirements.txt
```
**note** : Pour utiliser uv à terme on peut utiliser la  commande suivante

```cmd
    ud add -v requirements.txt
```

## `2- Configurer un environnement à partir de uv`

- Créer un environnement virtuel

- Installer les dépendances dans le uv.lock :
```cmd
    uv lock
```

## `3- Mettre à jour les dépendances`

```cmd
   uv lock -upgrade
```

## `4- Grouper les dépendances`

- Installer une dépendance dans un groupe .

**exemple**  :
```cmd
   uv add --group data_dep ipykernel
```


- Installer uniquement les dépendances principales :

```cmd
   uv sync --no-dev
```

## `5- Tool Management`

**exemple** : précision à uv de télécharger uniquement une version cpu de pytorch

```toml
[tool.uv.sources]

torch = { index = "pytorch-cpu" }

[[tool.uv.index]]

url = "https://download.pytorch.org/whl/cpu" explicit = true
```

# Contact
`Mail` : **maximeatsoudegbovi@gmail.com**
