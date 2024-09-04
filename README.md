# Git and Github Reference
This repository serves as a personal reference for Git and GitHub commands

## Basic Commands
* clone the repo to your computer
```bash
git clone [repo url]
```
* to see changes and files that modified or should be added to git
```bash
git status
```
* add file or files to git to be commited
```bash
git add [file | .]
```
* commit changes to git with a message and a description
```bash
git commit -m "message" -m "descripion"
```

## Setup SSH key
1. add your email inside the quotes insted of the example email
```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```
2. start the SSH agent by typing this command
```bash
eval "$(ssh-agent -s)"
```
3. add SSH private key to the SSH agent
```bash
ssh-add ~/.ssh/id_ed25519
```