This is my github test. I have added notes of the most used github commands which i can review on. 



1. git instanllation: 

 git init -> git branch -m main

2. set up configurations (global): 
 git config --global user.name "<myName>"
 git config --global user.email "<myEmail>"
 git config --global --list (check)
 git config --global init.defaultBranch main (set default branch)
 git config --global --unset (unset)

 3. basic local commands: 
 git status 
 git add <.>
 git commit -m "<commit message>"

 4. branch: 
 git branch <branch name>
 git branch -a (show all branch)
 git checkout <branch name>
 git checkout -b <branch name>

5. differences:
git diff
git diff --staged
git diff head b 

6. merge:
###############
checkout to main first then merge the other branch
###############
git merge <branch name> -m "<commit message>"

7. remote repositories:
git remote add origin <remote address> (for the first time)
git remote
git remote -v
git push -u origin <branch name> (for the first time)
git push <branch name>
git push

git clone <remote address>

git fetch -> git status -> git diff <branch name> origin/<branch name>
git pull

8. Vim editor hot keys: Type "i" to make changes, press <esc> to exit, type ":wq" to save and quit

9. conflicts and fix commits:
#############
fix the latest commit before push:
git commit --amend
#############

git log 
git log --oneline

git reset -- soft HEAD~<number of how many commits you want to reset back>                  (reset back to staged status)
git reset --mixed HEAD~<number of how many commits you want to reset back> = git reset      (reset back to tracked status)
git reset --hard HEAD~<number of how many commits you want to reset back>                   (###trash the new commits### reverse to older commits)

#############
find back trash commits:

git reflog (reflog only saved in local repository and it only last 90 days)

git cherry-pick <commits ID>
#############

