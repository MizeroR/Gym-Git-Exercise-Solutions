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
### Bundle 3 Exercise 1
```bash
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git branch ft/team-page
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi team.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git checkout main
M	README.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git branch ft/contact-page
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git branch   
  dev
  ft/bundle-2
  ft/contact-page
  ft/service-redesign
  ft/team-page
* main
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git checkout ft/team-page
M	README.md
Switched to branch 'ft/team-page'
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git log
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git cherry-pick fff8536f043b19a00da66695bb87cb7442040ea8
[ft/contact-page ce9af66] New heading in team page
 Date: Wed Dec 18 11:56:15 2024 +0200
 1 file changed, 1 insertion(+)
[ft/contact-page ce9af66] New heading in team page
 Date: Wed Dec 18 11:56:15 2024 +0200
 1 file changed, 1 insertion(+)
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git revert ce9af6672a2c6fc7373717ac896071f0218af6b4
[ft/faq-page 22ac245] Revert "New heading in team page" Revert This reverts commit ce9af6672a2c6fc7373717ac896071f0218af6b4.
 1 file changed, 1 deletion(-)
```
### Bundle 3 Exercise 2
```bash
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.
```
### Bundle 4 Exercise 1
```bash
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git remote add git-copy git@github.com:MizeroR/git-exercises.git
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git remote
git-copy
origin
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git push origin 
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git push git-copy
To https://github.com/MizeroR/git-exercises.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/MizeroR/git-exercises.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git pull
Already up to date.
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git pull git-copy
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 872 bytes | 218.00 KiB/s, done.
From https://github.com/MizeroR/git-exercises
 * [new branch]      main       -> git-copy/main
You asked to pull from the remote 'git-copy', but did not specify
a branch. Because this is not the default configured remote
for your current branch, you must specify a branch on the command line.
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git push
Everything up-to-date

```
### Bundle 4 Exercise 2
```bash
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git merge --squash ft/footer
Updating 98fc484..03c448f
Fast-forward
Squash commit -- not updating HEAD
 README.md   | 35 +++++++++++++++++++++++++++++++++++
 footer.html | 11 +++++++++++
 2 files changed, 46 insertions(+)
 create mode 100644 footer.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git commit -m 'footer changes squashing'
[ft/squashing a9638dd] footer changes squashing
 2 files changed, 46 insertions(+)
 create mode 100644 footer.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git push --set-upstream origin ft/squashing
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.15 KiB | 236.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/MizeroR/Gym-Git-Exercise-Solutions/pull/new/ft/squashing
remote:
To https://github.com/MizeroR/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/squashing -> ft/squashing
branch 'ft/squashing' set up to track 'origin/ft/squashing'.
```
