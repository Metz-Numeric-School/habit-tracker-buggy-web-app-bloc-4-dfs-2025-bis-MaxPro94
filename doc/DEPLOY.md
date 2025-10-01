# Procédure de Déploiement

Décrivez ci-dessous votre procédure de déploiement en détaillant chacune des étapes. De la préparation du VPS à la méthodologie de déploiement continu.

## Préparation du VPS
- Connexion au vps via ssh
- Installation de aaPanel Free sur le VPS
- Recuperation des login de aaPanel
- Desactivation de la fonction putenv appartenant a PHP, cela m'a empêcher d'installer correctement composer.

## Méthode de déploiement
- Accès à aaPanel via l'url donnée
- Choix de l'environnement : LNMP
- On point sur le dossier /public
- Attention à la réecriture NGINX, il faut l'ajouter à aaPanel sur le modèle mvc sinon nous aurons uniquement des 404 après la page d'accueil.
- Ajout du .env manuellement sur le projet avec les bonnes variables
- Création de la BDD via aaPanel
- Mise en place des tables via les fichiers .sql
