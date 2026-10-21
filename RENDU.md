## Modèle `RENDU.md`

```markdown
# Rendu : mimiphisto

- Dépôt : tp-git-qqch
- Site GitHub Pages : https://github.com/mimiphisto/tp-git-qqch/deployments/github-pages

## Ex2
git log --oneline : 
df1df9c (HEAD -> main, test/main) ex2 : corrige une faute
bb22c3c ex 2: ajoute trois lignes
866e5d1 ex2 : crée les notes
14aef5f ex1 : initialise le dépôt

## Ex3
- config.local est-il encore dans l'historique ? Pourquoi ?
config.local est encore dans l'historique car on l'a commité avant de le placer dans .gitignore par la suite. il existe dans le commit précédent.

## Ex4
- git status après avoir retiré brouillon.txt du staging :
On branch main
Your branch is ahead of 'test/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   README.md
	modified:   brouillon.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.DS_Store

no changes added to commit (use "git add" and/or "git commit -a")

- Différence entre annuler une modification et retirer du staging ?
Quand on retire du staging, la modification n'est pas perdue, elle n'est juste pas transmise pour le commit.

## Ex6
- À quoi servent <<<<<<<, ======= et >>>>>>> ?
<<<<< indique la version actuelle, === indique le conflit, >>>>> indique la fin de la version qu'on veut fusionner

## Ex7
- git stash list (avant récupération) :
stash@{0}: On main: ligne ex7
- Pourquoi annuler un commit plutôt que l'effacer de l'historique ?
il vaut mieux annuler un commit plutôt que de l'effacer pour garder une trace des modifications apportées, donc on ne réécrit pas l'historique.

## Ex8
- git pull = git fetch + quoi ?
git pull = git fetch (récupérer les nouveautés du dépôt distant sans fusionner) + git merge

## Ex10
git log --oneline --graph --all :
git log --oneline :
0d3be2e (HEAD -> main, tag: rendu) ex10 : compèete le rendu
b139a3a (test/main) ex9 : ajoute la page d'accueil
0d643e5 ex8 : modification depuis GitHub 2
66fb7e4 Merge branch 'main' of https://github.com/mimiphisto/tp-git-qqch
4337bfc erreur de moi
f7df252 ex8 : modification depuis GitHub
65ff63d Merge pull request #1 from mimiphisto/feature-contact
7da4d34 (test/feature-contact, feature-contact) ex8 : ajoute la page contact
0f0478c ex7 : ajoute la ligne en cours
d0818f6 Revert "ex7 : ajoute une ligne par erreur"
f747510 ex7 : ajoute une ligne par erreur
868a543 ex6 : résout le conflit du titre
e4b12fe (test/version-en) ex6 : titre en anglais
eef61ed (test/version-fr) ex6 : titre en français
04d4669 rendu exos 1 à 5
71a4d8d ex5 : fusionne feature-menu
70ecdbf (test/feature-menu) ex5 : ajoute un dessert
b1567d1 ex5 : crée le menu
a8196ed ex4 : supprime a-supprimer.txt
2eee186 ex4 : renomme ancien.txt
c5e1d12 ex4: ajoute trois fichiers
e8f964a ex3 : arrête de suivre config.local
3216a8a ex3: ajoute config.local (erreur)
4c1c4fc ex3 : ajoute .gitignore
df1df9c ex2 : corrige une faute
bb22c3c ex 2: ajoute trois lignes
866e5d1 ex2 : crée les notes
14aef5f ex1 : initialise le dépôt

git log --graph :
* commit 0d3be2eb8d2a511e862c5a9ecad9598daa8165b0 (HEAD -> main, tag: rendu)
| Author: mimiphisto <annabouffier08@gmail.com>
| Date:   Wed Oct 21 21:40:36 2026 +0200
| 
|     ex10 : compèete le rendu
| 
* commit b139a3a0e5cf38281dcea796668604846c18b9a4 (test/main)
| Author: mimiphisto <annabouffier08@gmail.com>
| Date:   Wed Oct 21 21:30:30 2026 +0200
| 
|     ex9 : ajoute la page d'accueil
| 
* commit 0d643e5aa7bf211e096204034d32badfe6236f12
| Author: Anna Bouffier <annabouffier08@gmail.com>
| Date:   Wed Oct 21 21:26:10 2026 +0200
| 
|     ex8 : modification depuis GitHub 2
|   
*   commit 66fb7e4ef9b36ae6971b66013eb47e463895b0db
|\  Merge: 4337bfc f7df252
| | Author: mimiphisto <annabouffier08@gmail.com>
| | Date:   Wed Oct 21 20:47:57 2026 +0200
| | 
| |     Merge branch 'main' of https://github.com/mimiphisto/tp-git-qqch
| | 
| * commit f7df25290ad65dd1f488827a29a6d42aabeba215
| | Author: Anna Bouffier <annabouffier08@gmail.com>
| | Date:   Wed Oct 21 20:35:54 2026 +0200
| | 

git log --all :
commit 0d3be2eb8d2a511e862c5a9ecad9598daa8165b0 (HEAD -> main, tag: rendu)
Author: mimiphisto <annabouffier08@gmail.com>
Date:   Wed Oct 21 21:40:36 2026 +0200

    ex10 : compèete le rendu

commit b139a3a0e5cf38281dcea796668604846c18b9a4 (test/main)
Author: mimiphisto <annabouffier08@gmail.com>
Date:   Wed Oct 21 21:30:30 2026 +0200

    ex9 : ajoute la page d'accueil

commit 0d643e5aa7bf211e096204034d32badfe6236f12
Author: Anna Bouffier <annabouffier08@gmail.com>
Date:   Wed Oct 21 21:26:10 2026 +0200

    ex8 : modification depuis GitHub 2

commit 66fb7e4ef9b36ae6971b66013eb47e463895b0db
Merge: 4337bfc f7df252
Author: mimiphisto <annabouffier08@gmail.com>
Date:   Wed Oct 21 20:47:57 2026 +0200

    Merge branch 'main' of https://github.com/mimiphisto/tp-git-qqch

commit 4337bfc0b69f9b2a1f0b6165bc7e7d57198766f6
Author: mimiphisto <annabouffier08@gmail.com>
Date:   Wed Oct 21 20:38:41 2026 +0200

git log --oneline --graph --all : (Bonus)
* eff265d (HEAD -> main, tag: rendu2) ex10 : complète le rendu
* 0d3be2e (tag: rendu) ex10 : compèete le rendu
* b139a3a (test/main) ex9 : ajoute la page d'accueil
* 0d643e5 ex8 : modification depuis GitHub 2
*   66fb7e4 Merge branch 'main' of https://github.com/mimiphisto/tp-git-qqch
|\  
| * f7df252 ex8 : modification depuis GitHub
* | 4337bfc erreur de moi
|/  
*   65ff63d Merge pull request #1 from mimiphisto/feature-contact
|\  
| * 7da4d34 (test/feature-contact, feature-contact) ex8 : ajoute la page contact
|/  
* 0f0478c ex7 : ajoute la ligne en cours
* d0818f6 Revert "ex7 : ajoute une ligne par erreur"
* f747510 ex7 : ajoute une ligne par erreur
*   868a543 ex6 : résout le conflit du titre
|\  
| * e4b12fe (test/version-en) ex6 : titre en anglais
* | eef61ed (test/version-fr) ex6 : titre en français
|/  
* 04d4669 rendu exos 1 à 5
*   71a4d8d ex5 : fusionne feature-menu
|\  
| * 70ecdbf (test/feature-menu) ex5 : ajoute un dessert
| * b1567d1 ex5 : crée le menu
|/  
* a8196ed ex4 : supprime a-supprimer.txt
* 2eee186 ex4 : renomme ancien.txt



https://github.com/mimiphisto/tp-git-qqch.git