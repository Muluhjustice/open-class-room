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