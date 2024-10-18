1Comment vérifier la configura�on actuelle de Git sur votre machine, notamment le nom
d’u�lisateur et l’adresse e-mail ?

git config --list
git config user.name
git config user.email

2Comment modifier votre adresse e-mail si vous l'avez mal configurée lors de l'installa�on
de Git ?
git config --global user.email "nouvelle-adresse@email.com"
git config user.email

3. Si vous avez oublié de créer un fichier README.md lors de l'ini�alisa�on du projet,
comment pouvez-vous l'ajouter après coup et commiter les changements ?
touch README.md
nano README.md
git add README.md
git commit -m "Ajout du fichier README.md"


4. Comment définir un dépôt distant si vous n'en avez pas configuré un lors de la créa�on
du projet ?
git remote add origin <URL>
git remote add origin https://github.com/utilisateur/nom_du_depot.git
git remote add origin git@gitlab.com:utilisateur/nom_du_depot.git
git remote -v
origin  https://github.com/utilisateur/nom_du_depot.git (fetch)
origin  https://github.com/utilisateur/nom_du_depot.git (push)
git push -u origin main

5. Comment annuler les modifica�ons locales d'un fichier avant de les ajouter à l'index ?

   git checkout -- <nom_du_fichier>

6. Comment visualiser les fichiers qui sont prêts à être commités dans Git (staging) ?
   
   git status
7. Comment suivre (track) un dépôt distant et récupérer toutes les branches de ce dépôt ?

   git remote add origin <URL_du_dépôt_distant>
git fetch origin
 git branch -a
git checkout -b <nom_de_la_branche_locale> origin/<nom_de_la_branche_distante>
8. Comment supprimer une branche locale après l'avoir fusionnée dans master ? git branch -d <nom_de_la_branche>

