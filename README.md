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

##Bundle 1 Exercise 2
'''bash

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

