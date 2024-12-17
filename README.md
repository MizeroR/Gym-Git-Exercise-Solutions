# Gym-Git-Exercise-Solutions
## List of commands used
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
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi home.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi about.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git stash
Saved working directory and index state WIP on main: 27400a1 New commands
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi about.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi team.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi team.html     
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git add team.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git stash
Saved working directory and index state WIP on main: 27400a1 New commands
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi team.html     
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % ls
README.md	about.html	file.txt	home.html	team.html
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

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{0} (7a7ea555e5851b04a728388f91bf660ed8a621fe)
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git add --all
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   about.html
	modified:   home.html
	modified:   team.html

mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git commit -m "Stashed files modification"
[main b58682c] Stashed files modification
 3 files changed, 34 insertions(+)
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git push
Enumerating objects: 9, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 694 bytes | 694.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/MizeroR/Gym-Git-Exercise-Solutions.git
   094bdf1..b58682c  main -> main
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git stash list
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git status
On branch ft/bundle-2
nothing to commit, working tree clean
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % vi services.html 
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git add services.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   services.html

mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git commit -m "Service page"
[ft/bundle-2 5dff588] Service page
 1 file changed, 11 insertions(+)
 create mode 100644 services.html
mizeroreine@Mizeros-MacBook-Air Gym-Git-Exercise-Solutions % git push 
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

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
