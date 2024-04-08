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


