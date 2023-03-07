
# Exercice 1 :  Clone a Git repository

## 3. Using only command-line in your Linux shell, clone it to a local repository.
```
git clone https://github.com/Lindaa25/TD7_GitBranches.git
```
# Exercice 2 :  Push files to common repository
## 1. Create a branch named after you.
```
cd TD7_GitBranches
git branch linda_he
```
## 2. Create a new text file named after you (with the content you want).
```
touch linda_he.txt
git add linda_he.txt
```
## 3. Commit this new file.
```
git commit -m "Ajout de mon fichier txt"
```
## 4. Push your branch to the remote repository.
```
git checkout linda_he
git push --set-upstream origin linda_he
git branch -a
```
token : dans github -> settings -> <developer settings> -> personal access token -> token classic -> generate (cocher reto)
  
# Exercice 3 : Merge simple changes
## 1. Merge your branch into the ’master’ branch.
```
git checkout linda_he
git merge main
```
## 2. Push your changes in the ’master’ branch to the remote repository.
  ```
  git push --set-upstream origin linda_he
  ```
  
# Exercice 4 : Resolve merge conflicts
  ## 1. Switch back to your own branch (not including the latest changes from the master branch).
  ```
  git checkout linda_he
  ```
  ## 2. Edit the lines 2 to 6 of the README.md file with a text you like
  ```
  nano README.md
  #crtl+O 
  #crtl+X
  ```
  
  ## 3. Commit this change
  ```
  git add README.md
  ```
  ## 4. Pull latest status from the remote repository ’master’ branch into your local ’master’ branch.
  ```
  git pull origin main
  ```
  ## 5. Merge your branch into the local ’master’ branch.
  ```
  git merge linda_he
  ```
  ## 6. If there are conflicts, we want the paragraph to appear in alphabetical order in the final README.md file
  ```
  sort linda_he.txt > linda_sorted.txt
  ```
  ## 7. Push your changes in the ’master’ branch to the remote repository.
  ```
  git push origin main
  ```
  
 # Exercice 5 :  Take latest changes from master in local branch
  
 ## 1. Pull the latest changes in the ’master’ branch, check the README.md
  ```
  git pull origin main
  ```
is up-to-date (contains all the paragraphs and the new line).
## 2. Switch back to your own branch (not including the latest changes from
the master branch).
```
git checkout linda_he
```
## 3. Merge the changes from ’master’ to your own branch.
```
git merge main
```
## 4. Commit this change 
```
git add README.md
git commit -m "Enregistrement effectué"
```
 # Exercice 6 : Delete a branch
  ## 1. Delete your branch on local repository.
  ```
  git branch -d linda_he
  ```
  ## 2. Delete your branch on distant repository.
  ```
  git push --delete origin linda_he
  ```
  
# Exercise 7: Rebase interactively to have a clean history
  
##Using only the shell in your local repository :
##1. Pull the latest changes in the ’master’ branch.
 ```
  $ git pull origin main
  ``` 
##2. Create a new local branch named after you and switch to it.  
 ```
  $ git checkout -b linda_he

  ```
  
 



