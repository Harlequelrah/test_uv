# **`Notes uv`**
Voici mes notes sur le cours uv de openclassroom.

**url** : **https://openclassrooms.com/fr/courses/8445356-gerez-votre-environnement-python-avec-uv**

# `Commandes uv`

## `1- Intitialisation  de uv`

```cmd
uv intit nom_du_projet
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
ou

    ```cmd
    ud add -v requirements.txt
    ```

**note** : Pour utiliser uv à terme on peut utiliser la deuxième commande



# Contact
`Mail` : **maximeatsoudegbovi@gmail.com**
