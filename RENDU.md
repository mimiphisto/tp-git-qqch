## Modèle `RENDU.md`

```markdown
# Rendu : mimiphisto

- Dépôt :
- Site GitHub Pages :

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

## Ex7
- git stash list (avant récupération) :
- Pourquoi annuler un commit plutôt que l'effacer de l'historique ?

## Ex8
- git pull = git fetch + quoi ?

## Ex10
git log --oneline --graph --all :
```