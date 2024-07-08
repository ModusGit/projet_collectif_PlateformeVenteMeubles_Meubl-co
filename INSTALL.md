# DOCUMENTATION POUR LE BACK

I. INSTALLER PHP : https://www.php.net/manual/fr/install.php
Sur MacOs,  et Linux télecharger avec Homebrew https://brew.sh/


II. INSTALLER COMPOSER, ici c'est detaillé pour tous les systèmes, il faut faire l'installation GLOBALE (c'est indiqué sur la doc)
https://getcomposer.org/doc/00-intro.md


III. INSTALLER SYMFONY
https://symfony.com/download 

Pour Debian/Ubuntu — APT based Linux :
curl -1sLf 'https://dl.cloudsmith.io/public/symfony/stable/setup.deb.sh' | sudo -E bash
sudo apt install symfony-cli

Pour MacOs :
1) Homebrew: install Homebrew https://brew.sh/
2) brew install symfony-cli/tap/symfony-cli

Pour Windows :
1) Installer Chocolatey (il faut s'inscire pour le télécharger)https://chocolatey.org/install c'est un gestionnaire de paquets qui va installer Symfony ou scoop, celui cité dans la doc Symfony: Scoop install Scoop
scoop install symfony-cli


IV. TUTOS
OFFICIELLE Symfony (for Dummies) tutos video : https://symfonycasts.com/
On conseille les chapitres : 1, 2, 3 et 8.

GRAFIKART
https://grafikart.fr/tutoriels/installation-symfony-2180#autoplay
On conseille fortement de gagner du temps, en regardant ces chapitres d'abord :
Découverte,
Installation,
Premières pages,
L'ORM doctrine,
ORM relation ManyToONe si on veux faire des tables relationnelles
Créer une API : le serializer, et suivre les autres si vous voulez aller plus loin


V. INSTALLER ADMINEREVO
Pour visualiser les bases de données, c'est un gestionnaire de basses de donnes GDBD
en français : https://download.adminerevo.org/4.8.4/adminer/adminer-mysql-fr.zip

Une fois téléchargé, le deziper, copier/coller dans le dossier public du projet et le renommer adminer.php avec l'explorateur de fichiers.


VI. PROJET
voici la doc officielle pour le framework Symfony
https://symfony.com/doc/current/setup.html


Dans le terminal, va dans le dossier où est le projet, écris cette ligne de commande :
$ composer require webapp

Vérifie que ton environement de travail est prêt avec: 
$ symfony check:requirements

ATTENTION le serveur XAMPP, LAMP, WAMP, MAMP doit être allumé pour faire tourner la base de donnée, mais il est inutile de mettre le projet dans htdocs.

Ouvre le projet, et sur le terminal, allume le serveur :
$ symfony server:start


NOTE : 
pour les problèmes de CORS (multisources otigins), il faut installer le bundle nelmio par composer avec la commande suivante dans le terminal :
composer require nelmio/cors-bundle
--> une fois installer s'assurer d'avoir sur votre Symfony votre fichier composer.json la ligne synfony/flex 
  - si oui, votre congiguration avec CORS gérés est fonctionnelle (plus besoin du plugins navigateurs anti-CORS) (documentations: https://github.com/nelmio/NelmioCorsBundle)
  - si non, vous trouvez cette ligne symfony/symfony, vous devez installer symfony/flex tel que : https://symfony.com/doc/current/setup/flex.html (suivre cette documentation)

# DOCUMENTATION POUR LE FRONT

- npm install -g create-react-app (installe Create React App mais ne marche pas)
- npm install react-bootstrap bootstrap (installe React Bootstrap)
- npm i react-router-dom (installe dépendances pour router)
- npm i mdb-react-ui-kit (pour installer le package de mise en forme card produit)
- npm start (pour lancer le projet)
