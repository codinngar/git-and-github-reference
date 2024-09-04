# Git and Github Reference
This repository serves as a personal reference for Git and GitHub commands

## Basic Commands

* Add git to an existing project:
```bash
git init
git remote add origin <repo ssh url>
```

* Clone a repo to your computer:
```bash
git clone <repo url>
```

* Show changes and files that modified or should be added to git:
```bash
git status
```

* Add file or files to git to be commited:
```bash
git add <file | .>
```

* Commit changes to git with a message and a description:
```bash
git commit -m "message" -m "descripion"
```

<br><br>

## Branching

* Show branches and the current branch:
```bash
git branch
```

* Add a new branch:
```bash
git branch <branch name>
```

* Create and switch to a new branch:
```bash
git checkout -b <branch name>
```

* Switch between branches:
```bash
git checkout <branch name>
```

* Show the difference between branches:
```bash
git diff <branch name>
```

* Merge a branch to the main one:
```bash
git checkout main # switch to the branch you want to merge another branch into it
git merge <branch name>
```

<br><br>

## Setup SSH key

1. Add your email inside the quotes insted of the example email:
```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

2. Start the SSH agent by typing this command:
```bash
eval "$(ssh-agent -s)"
```

3. Add SSH private key to the SSH agent:
```bash
ssh-add ~/.ssh/id_ed25519
```

4. Update the remote URL to SSH:
```bash
git remote set-url origin git@github.com:<username>/<repo name>.git
```

5. Check if the repo is using SSH now:
```bash
git remote -v
```