# touche-pas-au-klaxon
c'est une application qui permet d'optimiser le covoiturage au seins d'une entreprise qui a beaucoup de sites géographique
Parfois, plusieurs véhicules font le même trajet le même jour avec un taux d’occupation très faible
cette application servira donc à diffuser les trajets afin de pouvoir être mieux informé

$ FONCTIONNALITE

employé connecté :
- obtenir plus de détails sur un trajet
- Proposer un trajet
- Modifier, supprimer les trajets dont ils sont les auteurs.

administrateur:
-Tableau de bord
-supprimer n'importequel trajet
-Consulter la liste des utilisateurs
-Gérer la liste des agences

$TECHNIQUE
-PHP
-PHPmyadmin mySQL
-Apache via XAMPP
-Framework Bootstrap
- scss
-Dépendances : Composer

$INSTALLATION

Suivez ces étapes pour installer et lancer le projet sur votre machine locale.
Prérequis

 -XAMPP ou WampServer. (Cependant moi j'utilise XAMPP)

 -Composer installé globalement.

 -Git

1. Cloner le Dépôt

Ouvrez un terminal et placez-vous dans le dossier htdocs de votre installation XAMPP. Clonez ensuite le dépôt :

git clone https://github.com/BaptistePayan/touche-pas-au-klaxon.git touche-pas-au-klaxon
cd touche-pas-au-klaxon
code .

2. Installer les Dépendances

Lancer Composer pour installer les dépendances du projet (doit etre dejà installé en global sur la machine) :

composer install

3. Configurer l'Environnement

    À la racine du projet, créez un fichier nommé .env.

    Copiez le contenu suivant dans votre nouveau fichier .env et adaptez les valeurs si nécessaire (pour XAMPP par défaut, ces valeurs sont correctes) :

    # .env
    DB_HOST="localhost"
    DB_NAME="tpak_covoiturage"
    DB_USER="root"
    DB_PASS=""

4. Créer la Base de Données

    Démarrer les services Apache et MySQL depuis le panneau de contrôle XAMPP.

    Ouvrir votre navigateur et allez sur http://localhost/phpmyadmin.

    Créer une nouvelle base de données nommée tpak_covoiturage avec l'interclassement utf8mb4_general_ci.

    Sélectionner la base de données que vous venez de créer, allez dans l'onglet "Importer".

    Importer et exécutez le fichier src/sql/create_table.sql pour créer les tables.

    Importer et exécutez le fichier src/sql/seed.sql pour remplir les tables avec des données de test.

5. Lancer l'Application

L'application est maintenant prête ! Ouvrez votre navigateur et accédez à l'URL suivante :
http://localhost/touche-pas-au-klaxon/public/
👨‍💻 Utilisation

L'application est accessible à tous les visiteurs. Pour accéder aux fonctionnalités avancées, une connexion est nécessaire.
Identifiants de Connexion

Voici les comptes que vous pouvez utiliser pour tester l'application.
Compte Utilisateur Standard

    Email : jean.dupont@klaxon.com

    Mot de passe : password

Compte Administrateur

    Email : admin@klaxon.com

    Mot de passe : password
