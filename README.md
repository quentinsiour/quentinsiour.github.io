quentinsiour.github.io
======================

Clara Michel, Lucie Heslouis, Lucie Joulin, Quentin Siour, Asceline Boullen.

La procédure : 1. Installer une machine virtuelle 2. Dans votre machine virtuelle, aller dans «répertoire personnel » ou «home » et créer un dossier « sites » 3. Ouvrir un terminal dans votre machine virtuelle :

Mettre à jour les packets : sudo apt-get update entrez votre mot de passe de machine virtuelle

Vérifier qu'apache est démarré : sudo/etc/init.d/apache2 stop sudo/etc/init.d/apache2 start

Installer Ruby : http://michaelchelen.net/81fa/install-jekyll-2-ubuntu-14-04/ Les commandes pour installer ruby : sudo apt-get install ruby ruby-dev make faites « o » pour continuer pour vérifier : ruby -v la version doit être : 1.9.3p484

Installer Jekyll 2.4 qui dépend de Ruby sudo gem install jekyll jekyll -v la version est : 2.4 si message d'erreur : « could not find a Javascript run time » (https://github.com/joyent/node/wiki/installing-node.js-via-package-manager) sudo apt-get install nodejs

Installer Git, versionning la commande est sudo apt-get install git commande pour verifier : git -v puis tapez git version la version est alors : git version 1.9

Compte github github : https://pages.github.com/ Rendez-vous sur GitHub et créer un nouveau référentielnommé nom d'utilisateur .github.io, où nom d'utilisateur est votre nom d'utilisateur (ou nom de l'organisation) sur GitHub.
à droite du nom « + » > « create a repository » nommé .github.io
laissez public
cocher la case pour initialiser avec un readme.
faites sauver

Revenir sur la machine virtuelle

aller dans répertoire sites avec la commande cd sites
rogerdudler.github.io/git-guide/index.fr.html https://pages.github.com/ Cloner le dépôt
Faire la commande « cd sites » pour aller dans le répertoire sites
Allez dans le dossier où vous souhaitez stocker votre projet, et cloner le nouveau référentiel: ~ $ git clone https://github.com/ nom d'utilisateur / nom d'utilisateur .github.io

Entrez le dossier de projet et ajouter un fichier index.html: ~ $ cd nom d'utilisateur .github.io ~ $ echo "Hello world"> index.html

Ajouter/Modifier : (http://blog.alexis-hassler.com/2010/08/premiers-pas-avec-git-et-github.html) tapez les commandes : git init git config --global user.name "user" git config --global user.email « user@email.fr » ~ $ git add --all ~ $ git commit -m "commit initial" ~ $ git push

Tapez la commande « ls » pour vérifier que le index.html et readme.md se sont crées ou aller directement dans le dossier.
Tapez finalement la commande «git status » pour verifier si tout est a jour
Vous avez terminé!
Lancez un navigateur et allez à http: // nom d'utilisateur .github.io . Donnez-lui quelques minutes pour votre page apparaisse-il y aura un retard cette première fois.
