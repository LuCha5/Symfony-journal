# Journal en Ligne

Ce projet est une application de journal en ligne développée avec le framework Symfony. Elle permet de gérer des articles, auteurs et catégories, et offre une interface utilisateur intuitive avec un design épuré.

## Fonctionnalités

- **CRUD Complet** pour les entités :
  - **Articles** : ajout, modification, suppression, publication.
  - **Auteurs** : gestion des profils et des informations de l’auteur.
  - **Catégories** : classification des articles par catégorie.
- **Navigation intuitive** entre les différentes pages du site.
- **Recherche d'articles** avec filtres par auteur, date, et catégorie.
- **Enregistrement d'articles** pour lecture ultérieure.
- **Mode sombre et design responsive** pour un confort de lecture optimal.
  
## Prérequis

- **PHP** 8.1 ou supérieur
- **Composer** (pour la gestion des dépendances PHP)
- **Node.js et npm/yarn** (si tu utilises Webpack Encore pour gérer les assets)
- **Base de données** : MySQL, PostgreSQL, ou SQLite (selon configuration)

## Installation

### Étapes d'installation

1. **Cloner le dépôt**

   ```bash
   git clone https://github.com/LuCha5/Symfony-journal.git
   cd Symfony-journal
   ```

2. **Installer les dépendances PHP avec Composer**

   ```bash
   composer install
   ```

3. **Configurer les variables d’environnement**

   Duplique le fichier `.env` et configure-le en `.env.local`. Assure-toi de configurer la connexion à la base de données :

   ```
   DATABASE_URL="mysql://db_user:db_password@127.0.0.1:3306/db_name?serverVersion=5.7"
   ```

4. **Créer la base de données et exécuter les migrations**

   ```bash
   php bin/console doctrine:database:create
   php bin/console doctrine:migrations:migrate
   ```

5. **Démarrer le serveur de développement**

   ```bash
   symfony serve
   ```

   L’application sera accessible à [http://localhost:8000](http://localhost:8000).

## Utilisation

### Connexion et création d’articles

1. Accède à la page d'administration pour ajouter des **auteurs**, des **catégories** et des **articles**.
2. Chaque auteur peut gérer ses propres articles, les modifier, les publier, ou les enregistrer en brouillon.
3. Les utilisateurs peuvent consulter les articles par catégorie et utiliser le moteur de recherche pour filtrer les résultats.

## Technologies Utilisées

- **Symfony** : pour la structure back-end et le système d'ORM avec Doctrine.
- **Twig** : moteur de template pour le rendu des pages.
- **Webpack Encore** : gestion des assets et compilation des fichiers CSS et JavaScript.
- **Bootstrap** ou **CSS personnalisé** : pour le design responsive et minimaliste.
- **JavaScript (AJAX)** : pour les interactions en temps réel.

## Contribution

Les contributions sont les bienvenues ! Si tu souhaites améliorer ou corriger ce projet, ouvre une Pull Request.

1. Forke le projet.
2. Crée une branche pour ta fonctionnalité (`git checkout -b feature/nouvelle-feature`).
3. Commit tes modifications (`git commit -am 'Ajoute nouvelle fonctionnalité'`).
4. Push la branche (`git push origin feature/nouvelle-feature`).
5. Crée une Pull Request.

## Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.
