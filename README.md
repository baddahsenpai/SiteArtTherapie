# Site vitrine — Art-thérapie

Site statique en français pour promouvoir les services d'une art-thérapeute certifiée
(séances individuelles, ateliers de groupe, accompagnements pour troubles psychiques :
anxiété, stress, burn-out, deuil, traumatismes…).

## Structure

```
├── index.html            Accueil (hero, bienfaits, troubles accompagnés, déroulement)
├── art-therapie.html     Explication de l'art-thérapie
├── seances.html          Séances, tarifs et modalités pratiques
├── a-propos.html         Présentation de la praticienne et certification
├── contact.html          Formulaire de contact + infos pratiques
├── assets/
│   ├── css/style.css     Design sobre et apaisant, responsive
│   └── js/main.js        Menu mobile, année courante, feedback formulaire
└── README.md
```

## Personnalisation

À remplacer dans les pages HTML :

- `contact@exemple.fr` et `06 00 00 00 00` dans `contact.html` (formulaire en `mailto:`)
- L'adresse du cabinet et les horaires dans `contact.html`
- Les tarifs dans `seances.html`
- Le nom/prénom de la praticienne dans `a-propos.html`

Pour un envoi de formulaire sans `mailto:`, brancher le formulaire sur un service comme
Formspree, Netlify Forms ou un petit backend (modifier l'attribut `action` de
`<form>` dans `contact.html`).

## Mise en ligne

Aucune dépendance, aucun build : copier le contenu du dossier sur n'importe quel
hébergeur de site statique (GitHub Pages, Netlify, OVH, etc.) et ouvrir `index.html`.

## Test local

Ouvrir simplement `index.html` dans un navigateur, ou lancer :

```bash
python3 -m http.server 8000
```

puis visiter `http://localhost:8000`.
