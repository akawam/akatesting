# Test technique Akawam

Deux parties du projet sont présentes, Nuxtjs pour le site front & Laravel pour le backoffice/api.

Le projet est un blog très basique dans lequel on ajoute et on visualise des articles.

---
### Mise en place du projet


| Dépendance | Version |
| ------ | ------ |
| NodeJS | 12.x |
| PHP | 7.3 |

#### Dossier Laravel

- Installez les dépendances composer
- Installez les dépendances NPM avec Yarn ou NPM
- Compilez les fichiers CSS/JS
- Importez la base de données avec la commande `php artisan migrate --seed`
- Le domaine du projet doit être `akatesting.test`.

#### Dossier Nuxtjs

- Installez les dépendances NPM avec Yarn ou NPM
- Lancez le serveur avec la commande `yarn dev` ou `npm run dev`
- Visualisez le projet sur `localhost:3000`

---
### Objectifs

Le site doit afficher la liste des articles ajoutés depuis le backoffice laravel.
#### Global
- Faire tourner le projet sur votre environnement sans erreurs.
#### Laravel
- Ajouter la possibilité de supprimer & de modifier un article.
#### Nuxtjs
- Ajouter une bordure orange de 1px & une ombre aux articles grâce aux classes tailwindCss.

---
### Objectifs bonus

#### Laravel
- Ajouter un auteur aux articles

#### Nuxtjs
- Créer la page derrière le bouton "Voir l'article"

#### ++++
- Si vous avez tout fait et que vous avez encore du temps, changer/ajouter tout ce que vous trouverez pertinent.
