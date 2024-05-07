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
