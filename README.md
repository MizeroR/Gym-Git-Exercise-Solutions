# Gym-Git-Exercise-Solutions
## List of commands used
## Bundle 1 Exercise 1
1. mkdir Gym-Git-Exercise-Solutions
2. cd Gym-Git-Exercise-Solutions
3. vi README.md
4. vi index.html
5. echo hello > file.txt
6. echo world >> file.txt
7. git commit -am (to commit all modified content)
8. git push
9. git branch dev (to create a new branch)
10. git checkout dev (to switch branch)
11. git branch test(to create new branch)
12. git checkout -b test dev (to create a sub branch)
13. git branch -d test (to delete branch)
14. git checkout main (switched to main branch)

## Bundle 1 Exercise 2

```bash

mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi home.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi home.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git add .
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi home.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git stash
Saved working directory and index state WIP on main: 27400a1 New commands
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi about.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git add about.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi about.html     
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi home.html      
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git branch
  dev
* main

mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git stash list
stash@{0}: WIP on main: 27400a1 New commands
stash@{1}: WIP on main: 27400a1 New commands
stash@{2}: WIP on main: 27400a1 New commands
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git stash pop stash@{2}
Auto-merging home.html
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{2} (9849a2e5274d881ea1ff3dcd57f91b6d85c2cd51)
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi home.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git stash pop stash@{1}
Auto-merging about.html
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   about.html
	modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{1} (6ac0a2259bac0a02f92ef58b2900622f97b4cd17)
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git stash pop stash@{0}
Auto-merging team.html
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   about.html
	modified:   home.html
	modified:   team.html

mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git stash list
```
## Bundle 2 Exercise 1
```bash
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git status
On branch ft/bundle-2
nothing to commit, working tree clean
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git push --set-upstream origin ft/bundle-
error: src refspec ft/bundle- does not match any
error: failed to push some refs to 'https://github.com/MizeroR/Gym-Git-Exercise-Solutions.git'
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 436 bytes | 218.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/MizeroR/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote: 
To https://github.com/MizeroR/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```
### Bundle 2 Exercise 2
```bash
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi README.md
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi services.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git add services.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git commit -m 'Services'
[ft/service-redesign ec3e90a] Services
 1 file changed, 3 insertions(+)
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions %  git push origin ft/service-redesign
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git checkout ft/service-redesign
Already on 'ft/service-redesign'
Your branch is behind 'origin/main' by 2 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git merge main
Updating ec3e90a..ae6b19c
Fast-forward
 README.md     | 10 ++++++++++
 services.html |  1 +
 2 files changed, 11 insertions(+)
```
