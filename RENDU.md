## Modèle `RENDU.md`

```markdown
# Rendu : el-champiignon

- Dépôt : https://github.com/el-champiignon/tp-git-1
- Site GitHub Pages : [el-champiignon.github.io/tp-git-1/](https://el-champiignon.github.io/tp-git-1/)

## Ex2
git log --oneline :
a097ffb (HEAD -> main, origin/main) ex2: corrige une faute
ecaed53 ex2: ajoute trois lignes
17d59bb ex2: crée les notes
63377ca ex1: initialise le dépôt


## Ex3
- config.local est-il encore dans l'historique ? Pourquoi ? Il n'y est plus car git l'ignore.

## Ex4
- git status après avoir retiré brouillon.txt du staging : 
 Sur la branche main
Votre branche est en avance sur 'origin/main' de 3 commits.
  (utilisez "git push" pour publier vos commits locaux)

Modifications qui ne seront pas validées :
  (utilisez "git add <fichier>..." pour mettre à jour ce qui sera validé)
  (utilisez "git restore <fichier>..." pour annuler les modifications dans le répertoire de travail)
	modifié :         RENDU.md
	modifié :         brouillon.txt

Fichiers non suivis:
  (utilisez "git add <fichier>..." pour inclure dans ce qui sera validé)
	.gitignore

aucune modification n'a été ajoutée à la validation (utilisez "git add" ou "git commit -a")

  
- Différence entre annuler une modification et retirer du staging : quand on annule une modification, on peut en retrouver la trace dans l'historique. Quand on retire du staging, on arrête de traquer et on ne peut plus retrouver les modifications avec git.

## Ex6
- À quoi servent <<<<<<<, ======= et >>>>>>> ? A marquer les conflits entre fichiers : << la branche actuelle, == séparation entre les branches, >> les changements de la branche qu'on veut merge.

## Ex7
- git stash list (avant récupération) :
 stash@{0}: WIP on main: 61ef857 Revert "ex7: ajoute une ligne par erreur"

- Pourquoi annuler un commit plutôt que l'effacer de l'historique ? Pour garder un historique consistant, particulièrement utile si on est plusieurs à travailler sur un même projet. 

## Ex8
- git pull = git fetch + git merge

## Ex10
git log --oneline --graph --all :

* 6417b2f (HEAD -> main, origin/main, origin/HEAD) ex9: ajoute la page d'accueil
* 47b366e Update README.md
*   80bd95a Merge pull request #1 from el-champiignon/feature-contact
|\  
| * 0eb7aef (origin/feature-contact, feature-contact) ex8: ajoute la page contact
|/  
* d07ce13 ex7: ajoute la ligne en cours
| * 58265ed (refs/stash) WIP on main: 61ef857 Revert "ex7: ajoute une ligne par erreur"
|/| 
| * 02c36cd index on main: 61ef857 Revert "ex7: ajoute une ligne par erreur"
|/  
* 61ef857 Revert "ex7: ajoute une ligne par erreur"
* 5034aeb ex7: ajoute une ligne par erreur
* 9de3142 Revert "ex7: ajoute une ligne par erreur"
* 7dc0be4 ex7: ajoute une ligne par erreur
*   2ec223f ex6: résout le conflit du titre
|\  
| * c91c68d (origin/version-en) ex6: titre en anglais
* |   d6a37df Merge branch 'version-fr'
|\ \  
| |/  
:...skipping...
* 6417b2f (HEAD -> main, origin/main, origin/HEAD) ex9: ajoute la page d'accueil
* 47b366e Update README.md
*   80bd95a Merge pull request #1 from el-champiignon/feature-contact
|\  
| * 0eb7aef (origin/feature-contact, feature-contact) ex8: ajoute la page contact
|/  
* d07ce13 ex7: ajoute la ligne en cours
| * 58265ed (refs/stash) WIP on main: 61ef857 Revert "ex7: ajoute une ligne par erreur"
|/| 
| * 02c36cd index on main: 61ef857 Revert "ex7: ajoute une ligne par erreur"
|/  
* 61ef857 Revert "ex7: ajoute une ligne par erreur"
* 5034aeb ex7: ajoute une ligne par erreur
* 9de3142 Revert "ex7: ajoute une ligne par erreur"
* 7dc0be4 ex7: ajoute une ligne par erreur
*   2ec223f ex6: résout le conflit du titre
|\  
| * c91c68d (origin/version-en) ex6: titre en anglais
* |   d6a37df Merge branch 'version-fr'
|\ \  
| |/  
|/|   
| * 8d6dac9 (origin/version-fr) ex6: titre en français
|/  
*   5b27e25 ex5: fusionne feature-menu
|\  
| * ed66077 (origin/feature-menu) ex5: ajoute un dessert
| * ac44a23 ex5: crée le menu
|/  
* 00bafb7 ex4: supprime a-supprimer.txt
* 637c2e2 ex4: renomme ancien.txt
* 57217ca ex4: ajoute trois fichiers
* 292ccec ex3: arrête de suivre config.local
* ab98014 ex3: ajoute config.local (erreur)
* a097ffb ex2: corrige une faute
* ecaed53 ex2: ajoute trois lignes
* 17d59bb ex2: crée les notes
* 63377ca ex1: initialise le dépôt



```
