# repertoire-action
Un template pour que les militants puissent lister des actions inspirantes pour aider les gens à passer à l’action

## Contenu du dépôt

- `action.html` — page principale pour lister les actions.
- `detail.html` — page de détail pour afficher/modifier une action individuelle.
- `actions.json` — données JSON contenant la liste des actions.

## But

Fournir une interface simple (HTML/JS) pour visualiser et modifier des actions stockées dans `actions.json`.

## Ouvrir le projet

1. Ouvrez le dossier dans votre éditeur (VS Code, etc.).
2. Servez les fichiers statiques via un serveur local (préféré) ou ouvrez les fichiers directement dans le navigateur.

Exemple rapide avec Python 3 (macOS / Linux) depuis la racine du projet :

```bash
python3 -m http.server 8000
```

Puis ouvrez http://localhost:8000/action.html

> Remarque : si `actions.json` est chargé via fetch/XHR, ouvrir `action.html` directement avec le protocole `file://` peut empêcher le chargement en raison de restrictions CORS; utiliser un serveur local.

## Modifier `actions.json`

- Le fichier `actions.json` contient un tableau d'objets action. Sauvegardez une copie avant d'éditer.
- Exemple d'entrée :

```json
[
  {
    "id": 1,
    "titre": "Voter",
    "facilite": "Facile",
    "echelle": "Collectif",
    "rapidite": "Rapide",
    "description": "Voter lors d’élection permet de choisir les dirigeants."
  }
]
```

Pour vous faciliter la vie, voici un Google Sheets avec l'ensemble des actions : https://docs.google.com/spreadsheets/d/1juOJRkG37JeHqQ73Mpt0cjn7Fcl1YHma-_876gMpe5k/edit?usp=sharing 
1. Faites une copie,
2. Faites les modifications que vous souhaitez,
3. Enregistrez en CSV puis
4. Trouvez un convertisseur CSV to JSON
5. Renommez en actions.json
6. Remplacez le fichier actions.json du projet

## Modifier `logo.png`

- Ajoutez votre propre logo.png
