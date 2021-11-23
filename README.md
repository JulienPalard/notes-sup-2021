https://en.wikipedia.org/wiki/Markdown 
 
# Vocabulaire

On utilise un shell (bash, fish, zsh, ...), qui interprête nos commandes. Le shell s'affiche dans un « émulateur de terminal » (on pronocera juste *terminal*), c'est la fenêtre qui émule un vieux [VT100](https://fr.wikipedia.org/wiki/VT100).


# Commandes shell

## `pwd` [Print Work Directory]

Voir où on se situe dans nos dossiers.

## `cd` [Change Directory]

Pour se déplacer dans un dossier.

`cd -` = revenir dans le dossier où on se situait juste avant
`cd ..` = aller dans le dossier parent.
`cd` = aller dans son dossier personnel.

## `ls` [List]

Pour lister les fichiers et dossiers du dossier où on se trouve.
* `ls` = liste classique.
* `ls -l` = liste en vertical avec plusieurs informations supplémentaires.
* `ls -h` = afficher la taille des fichiers dans la liste en Ko/Mo/Go...
* `ls -a` = afficher tous les dossiers, même ceux qui sont cachés.
* `ls *.exemple` = liste de tous les fichiers qui termine par .exemple


## `man` [Manual]

Afficher le manuel d'informations d'un élément.
* `man -k mot` = rechercher tous les manuels contenant le mot entré après le -k.

## `cp` [Copy]

Copier coller un fichier/dossier d'un endroit à un autre.
* `cp .../.../ .` = copie colle le fichier rechercher à l'endroit où on se trouve.
* `cp fichier_a fichier_b` = copie le fichier_a vers le fichier_b (qui peut ne pas encore exister et être crée pour l'occasion)

## `mv` [Move]

Déplacer un fichier/dossier.
* `mv exemple.html exemple.txt` = mv déplace et/ou modifie le nom/l'extension d'un fichier ou d'un dossier.


## `rm` [Remove]

Supprime un dossier/fichier **définitivement** (pas de corveille (faites vos sauvegardes)).
* `rm -rf le_dossier` = supprime un dossier non vide.
* `rm un_fichier` = supprime un fichier



## `grep` [Global REgex Print]

Cherche un mot dans les lignes du fichier
    * `grep 163.5.68.1 /var/log/nginx/access.log` = cherche les accès d'une IP dans un fichier de log

petite modification