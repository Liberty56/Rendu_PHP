# Projet Portfolio - Gestion des Utilisateurs et des Compétences

## Présentation du Projet
Ce projet est une application web développée en PHP & MySQL permettant aux utilisateurs de :
- [ ] Gérer leur profil (inscription, connexion, mise à jour des informations).
- [ ] Ajouter et modifier leurs compétences parmi celles définies par un administrateur.
- [ ] Ajouter et gérer leurs projets (titre, description, image et lien).
- [ ] Un administrateur peut gérer les compétences disponibles.

## Fonctionnalités Implémentées

### Authentification & Gestion des Comptes
- [ ] Inscription avec validation des champs
- [ ] Connexion sécurisée avec sessions et option "Se souvenir de moi"
- [ ] Gestion des rôles (Admin / Utilisateur)
- [ ] Mise à jour des informations utilisateur
- [ ] Réinitialisation du mot de passe
- [ ] Déconnexion sécurisée

### Gestion des Compétences
- [ ] L’administrateur peut gérer les compétences proposées
- [ ] Un utilisateur peut sélectionner ses compétences parmi celles disponibles
- [ ] Niveau de compétence défini sur une échelle (débutant → expert)

### Gestion des Projets
- [ ] Ajout, modification et suppression de projets
- [ ] Chaque projet contient : Titre, Description, Image, Lien externe
- [ ] Upload sécurisé des images avec restrictions de format et taille
- [ ] Affichage structuré des projets

### Sécurité
- [ ] Protection contre XSS, CSRF et injections SQL
- [ ] Hachage sécurisé des mots de passe
- [ ] Gestion des erreurs utilisateur avec affichage des messages et conservation des champs remplis
- [ ] Expiration automatique de la session après inactivité

## Installation et Configuration
- Lancer les modules Apache et MYSQL avec XAMPP
- Run le code
- Pour accéder aux pages "Projet" et "Vos compétences", il faut le faire directement dans la barre de recherche (ex: localhost:8000/Projet.php)
### Prérequis
- Serveur local (XAMPP, WAMP, etc.)
- PHP 8.x et MySQL
- Un navigateur moderne

### Étapes d’Installation
1. Cloner le projet sur votre serveur local :
   ```sh
   git clone url_de_votre_repo
   cd nom_projet_a_renseigner
   ```
2. Importer la base de données :
   - ici le fichier data.sql

3. Configurer la connexion à la base de données :
   Modifier le fichier `config/database.php` :
   ```php
   define('DB_HOST', 'localhost');
   define('DB_NAME', 'projet_web');
   define('DB_USER', 'projet_web');
   define('DB_PASS', 'password');
   define('DB_PORT', 3306);
   ```
   Puis accéder à l'application via `http://localhost:8000`

## Comptes de Test
- bob@mail.com
- password
### Compte Administrateur
- **Email** : admin@example.com
- **Mot de passe** : password

### Compte Utilisateur
- **Email** : user@example.com
- **Mot de passe** : password

## Structure du Projet
PHP:
   -config:
      -connexion.php,
      -database.sql,
   -uploads:
      -(image des projets),
   -A propos de moi.php,
   -Accueil2.php,
   -data.sql,
   -Inscription.php,
   -Login.php,
   -Logout.php,
   -profil.png (bonhomme sur l'accueil),
   -Projet.php,
   -Style2.css,
   -Vos compétences.php

## Licence
Ce projet est sous licence MIT.

## Contact
Une question ou un bug ? Contactez-moi : mon.email@example.com
