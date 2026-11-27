# MonSiteWeb

Site vitrine statique en HTML/CSS, réalisé dans le cadre d'un cours Git et GitHub. Il sert de fil rouge pour apprendre le versionnage : commits, branches, Pull Requests, résolution de conflits, tags et releases.

## Contenu du site

- En-tête avec le titre et la navigation (À propos, Services, Contact)
- Section À propos
- Section Nos services
- Section Témoignages
- Section Contact
- Pied de page

## Technologies

- HTML5
- CSS3
- Git et GitHub

## Structure du projet

    MonSiteWeb/
    ├── index.html
    ├── style.css
    ├── .gitignore
    └── README.md

## Lancer le projet

Aucune installation n'est nécessaire.

    git clone https://github.com/nodemnodemlucaevans/MonSiteWeb.git
    cd MonSiteWeb

Ouvrir ensuite le fichier `index.html` dans un navigateur.

## Organisation du travail avec Git

- La branche `main` contient la version stable du site.
- Chaque modification se fait sur une branche dédiée, puis passe par une Pull Request avant d'être fusionnée.
- Un commit correspond à un seul changement cohérent, avec un message clair.

### Convention des messages de commit

Format : `type: description courte`

| Type | Usage | Exemple |
|------|-------|---------|
| feat | Nouvelle fonctionnalité | feat: ajouter la section témoignages |
| fix | Correction d'une erreur | fix: corriger les liens du menu |
| docs | Documentation | docs: ajouter le README du projet |
| style | Mise en forme du code | style: améliorer les espacements |
| refactor | Réorganisation sans changer le résultat | refactor: simplifier le CSS |
| chore | Entretien et configuration | chore: ajouter le fichier gitignore |

## Historique du projet

| Étape | Description |
|-------|-------------|
| Commit initial | Structure HTML et CSS du site |
| PR #1 | Ajout de la section Témoignages (branche `ajout-temoignages`) |
| PR #2 | Couleur rose pour l'en-tête (branche `couleur-rose`) |
| PR #3 | Couleur bordeaux pour l'en-tête (branche `couleur-bordeaux`) |
| Tag v0.1.0 | Première version de démonstration |

## Simulation d'un conflit en équipe

Deux collaborateurs ont modifié la même ligne de `style.css` (la couleur de fond de l'en-tête), chacun sur sa propre branche : rose d'un côté, bordeaux de l'autre.

1. La Pull Request #2 (rose) a été fusionnée en premier.
2. La Pull Request #3 (bordeaux) est alors entrée en conflit : Git ne pouvait pas choisir entre les deux couleurs.
3. Le conflit a été résolu en fusionnant `main` dans la branche bordeaux, en repérant les marqueurs `<<<<<<<`, `=======` et `>>>>>>>`, en choisissant la couleur finale et en supprimant les marqueurs.
4. Un commit de résolution a ensuite été poussé, et la Pull Request a pu être fusionnée.

## Versions

Le projet suit le versionnage sémantique MAJOR.MINOR.PATCH.

- `v0.1.0` : première version de démonstration

## Équipe

- nodemnodemlucaevans : propriétaire du dépôt
- Kamta Yann (Davys-STARK) : collaborateur
