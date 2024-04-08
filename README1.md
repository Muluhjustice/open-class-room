-Un gestionnaire de versions est un programme qui permet aux développeurs de conserver un historique des modifications et des versions de tous leurs fichiers.
-git est utiliser en local et github est utiliser en ligne
-Git est un gestionnaire de versions. Vous l’utiliserez pour créer un dépôt local et gérer les versions de vos fichiers.

-GitHub est un service en ligne qui va héberger votre dépôt. Dans ce cas, on parle de dépôt distant puisqu’il n’est pas stocké sur votre machine.
-Un dépôt est comme un dossier qui conserve un historique des versions et des modifications d’un projet. Il peut être local ou distant
-un dépôt local est un entrepôt virtuel de votre projet. Il vous permet d'enregistrer les versions de votre code et d'y accéder au besoin
un depot distant:Il permet de stocker les différentes versions de votre code afin de garder un historique délocalisé, c'est-à-dire un historique hébergé sur Internet ou sur un réseau
confuguration de l'identite: en utilisant la command :git config --global user.name "name"
-git config --global user.email "email" 
pour verifier si les parametre a ete bien cree il suffit de passer la command :git config --list
configurez les couleur :git config --global color.diff auto $ git config
 --global color.status auto $ git config --global
 color.branch auto
configurez les editeur :git config --global core.editor notepad++ $ git config 
--global merge.tool vimdiff
-creer le dossier quont soit travaller avec la command mkdir (nom du fichier)
         

  -Touch (the name of the file): permits to creat a new file in cmmand line and it can be seen in our folder
 -git permits to see if the file was created
 -git add (name) :permits files in git index
 -git commit: permits to creates a new verson of the project and it passes the commandes which are in the stage in the reporistories
 e.g git commit -m "message"
 - to add the styles.css to index.html we can use the command
 * touch Styles.css 
 * git add index.html style.css


 Before sending the code to github we will have to create and generate a private and public key
 -ssh-keygen permits to generate a private and public key 
 *by using ssh-keygen -t et25519 -C "email.addres" permits githube to authentify you in every action
 -to copy the public key to our press paper we can use the command (clic < ~/.ssh/id_github_ed25519.pub)

 -git remote add:
origin git@github.com:EtudiantOC/OpenclassroomsProject.git
-to connect the depot local to the distant depot we use the command git branch -M main
-git push -u origin main permits to send the commits on a distant github(online cloude)
  les branche
- this are copies of the original files and can be tested without affecting the the initial code

git branch :to know the branch present in a project

git branch cagnotte: elle cree une branche en local
ensuit un git branch
git checkout cagnotte: permets de basculer la branch
git commit -m : pour enregistre les modification avec les description du message en local
git push origin (nom de la branch): permet de envoyer les modification sur le depot distant githube
git merge (nom de la branch): permet la fusion de deux branch
git clone (url de ssh dans githube)

git pull origin main: permet de rappeler le projet en local

git branche : permet de voir si les branch a ete cree



git branch -d (nom de la branch): permet de suprimer la branch quont vien de cree
git branch -D : Permet la suppression de la branch specifier
git satus: permets de voir les differnt index qui ont ete cree et ceux qui nont pas ete cree
git stash: permet de mettre en attent les modification local no valide et de partir sur une autre branch
git stash apply: applique les modification du dernier  stash qui a ete fait
git stash list : permet de voir les different stash qui ont ete mise en attent
git stash apply (nom du stash): s va applique les different modification
 git log: liste les different commit qui ont ete effectue
 git reset --hard HEAD^: CETTE  commande va supprimer de la branche principale votre dernier commit.  Le HEAD^ indique que c'est bien le dernier commit que nous voulons supprimer. L’historique sera changé, les fichiers seront supprimés
 *cree une nouvel branch(git branch (nom de la branch))
 *bascule cette branch (git checkout branch et applique les differnt commitskout nom de la branch)
 -git reset: permet de renouvellr branch et applique les differnt commit
 *git reset --hard (identifiant)
 git commit --amend -m "":  Cette commande va fonctionner pour le dernier commit réalisé ! Lorsque l'on travaille sur un projet avec Git, il est très important de marquer correctement les modifications effectuées dans le message descriptif.
 git add FichiereOblie.txt
 git commit --amend -- no_edid: Votre fichier a été ajouté à votre commit et grâce à la commande
 git revert : cree un nouveau cummit
 git revert head:
 git blame: permet de voir qui a fait une modification sur une ligne precise
 git branch -r :Si la branche a été push il y a un moment, elle devient stale, c’est-à-dire qu’elle est considérée comme inactive et GitHub ne la retourne plus da ns la liste. Pour résoudre ce problème, lancez la commande suivante :