# Documentation for AGV Git Task

## Task 1

Solution: \
(Unnecessary and erroneous commands that were mistakenly entered in the Terminal are omitted)

```bash
gh repo fork --clone --remote=false Cath3dr4l/AGV-git-task
cd AGV-git-task
git checkout -b "Task1"
vim README.md #Do the required changes here
git add .
git commit -S -m "Added my name(Sandip Das) to the list of Entries"
git push https://github.com/real-Sandip-Das/AGV-git-task Task1
gh pr create --base main --head real-Sandip-Das:Task1 --title "Task1: Added entry to README.md" --body "Added Name, GitHub username and link to Github account as mentioned"
```

Screenshots:

![1. Creating a Fork(left configuring remote for Task 3)](Images/Task%201/Fork.png)

1: Creating a Fork(using the GitHub CLI, left remote configuration for Task 3)

![2. Creating the Branch 'Task1'](Images/Task%201/Branching.png)

2: Creating the Branch 'Task1'

![3. Modifying Files, Committing Changes(with SSH Signing, the '-S' flag that results in the green 'Verified' sign being shown while my commit is viewed on github.com), Pushing to remote](Images/Task%201/Commit_Push.png)

3: Modifying Files, Committing Changes(with SSH Signing, the '-S' flag that results in the green 'Verified' sign being shown while my commit is viewed on github.com), Pushing to remote

(like this:)

![Verified](Images/Task%201/Verified.png)

![4. Creating the pull request(again, using the GitHub CLI)](Images/Task%201/PullReq.png)

4: Creating the pull request(again, using the GitHub CLI)

## Task 2

Solution:

```bash
git remote add origin https://github.com/real-Sandip-Das/AGV-git-task.git
git remote -v
#TODO: complete the task
```

Configuring remote:
![Adding remote](Images/Task%202/adding_remote.png)

## Task 3

Solution:

```bash
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
git checkout -b "Task3"
vim dummy-main.cpp #added some dummy code
git add .
git commit -S -m "Added some code, hope it works and passes all the Tests😁"
git revert Task3 #GNU Nano opens up for editing the commit message
git push origin Task3
gh pr create --base main --head real-Sandip-Das:Task3 --title "Task3: Sandip Das" --body "Pull request for Task 3"
```

![Screenshot](Images/Task%202/image.png)

## Task 4

Solution:

```bash
git checkout -b "Task4"
vim dummy-main.cpp #Added some stupid code
git add .
git commit -S -m "Added a new file!"
#Now realized that I've done something stupid
git reset --hard Task4^
```

![Screenshot](Images/Task%204/image.png)

## Task 5

Solution:

```bash
git checkout main
git fetch upstream
git merge upstream/main
git push origin main

git checkout -b "Task5"
vim main.cpp
git add .
git commit -S -m "Added dummy code, first time"
vim main.cpp
git add . && git commit -S -m "Added dummy code, second time"
vim main.cpp
git add . && git commit -S -m "Added dummy code, third time"
vim main.cpp
git add . && git commit -S -m "Added dummy code, fourth time"
vim main.cpp
git add . && git commit -S -m "Added dummy code, fifth time"
vim main.cpp
git add . && git commit -S -m "Added dummy code, sixth time"
git rebase --interactive Task5~6
#drop second and fourth commits in the text editor
#merge conflicts if asked to

git push origin Task5
gh pr create --base main --head real-Sandip-Das:Task5 --title "Task5: Added dummy code multiple times and removed the 2nd and 4th commits (Sandip Das)" --body "Added Dummy code six times and removed(a.k.a. 'drop'ped) the second and fourth commits using Interactive Rebase"
```

Selecting commits in vim: \
![Vim initial](Images/Task%205/vim_initial.png) \
![Vim Final](Images/Task%205/vim_final.png)

Screenshots of terminal: \
![Terminal](Images/Task%205/task5terminal.png) \
![Terminal 2](Images/Task%205/task5terminal2.png)
