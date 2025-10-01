# Procédure de Déploiement

Décrivez ci-dessous votre procédure de déploiement en détaillant chacune des étapes. De la préparation du VPS à la méthodologie de déploiement continu.

## Préparation du VPS
- Connexion au vps via ssh
- Installation de aaPanel Free sur le VPS
- Recuperation des login de aaPanel.
- Accès à aaPanel via l'url donnée suite à l'installation : https://172.17.4.22:32604/92647feb
- Desactivation de la fonction putenv appartenant a PHP. Cela m'a empêcher d'installer correctement composer via CLI.
- Choix de l'environnement : LNMP
- On pointe sur le dossier /public
- Attention à la réecriture NGINX, il faut l'ajouter à aaPanel sur le modèle de réecriture mvc sinon nous aurons uniquement des 404 après la page d'accueil.
- Création de la BDD via aaPanel et les scripts fournis.
- Ajout du .env manuellement sur le projet avec les bonnes variables.

## Méthode de déploiement
- Correction en local pour les erreurs et modifications.
- Commit a chaque problème resolu ou modification importante.
- Une fois les problèmes resolus je crée un tag ex: 1.1.1
- Je push le tout sur mon repository.
- Je met a jour le VPS en m'appuyant sur le dernier tag ( version stable ) pour la MàJ.
