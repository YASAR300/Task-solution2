name


# Git Notes: Comprehensive Overview with Explanations

## Part 1: Git Basics

### Task 1: Install and Configure Git
**What to do**: Install Git and configure it to associate commits with your name and email.

#### Steps:
1. Install Git from [git-scm.com](https://git-scm.com/).
2. Configure your username and email:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your-email@example. com"
   ```

- Verify configuration:
   ```bash
    git config --list
    ```
## Task 2: Initialize a Repository
- Create and initialize a directory as a Git repository:
  ```bash

    mkdir MyProject
    cd MyProject
    git init
    ```
- Purpose: Creates a .git folder to track changes.
# Part 2: Basic Workflow
## Task 3: Creating and Committing Files
- Create a file:
 ```bash

 echo "Hello Git" > file1.txt
 ```
- Stage and commit:
 ```bash

 git add file1.txt
 git commit -m "Initial commit: Added file1.txt"
 ```
## Task 4: Viewing Changes
- Modify the file:
 ```bash

echo "Git is awesome!" >> file1.txt
```
- Check status and differences:
 ```bash

git status
git diff
```
## Task 5: Undoing Changes
- Unstage a staged file:
 ```bash

git reset file1.txt
```
- Discard uncommitted changes:
 ```bash

git checkout -- file1.txt
 ```
# Part 3: Branching and Merging
## Task 6: Branch Management
- Create a new branch:
 ```bash

git checkout -b feature-branch
 ```
- List branches:
 ```bash

git branch
 ```
- Rename a branch:
 ```bash

git branch -m feature-branch feature-enhanced
 ```
## Task 7: Merging Branches
- Merge a branch into the main branch:
 ```bash

 git checkout main
git merge feature-enhanced
 ```
## Task 8: Handling Merge Conflicts
- Resolve conflicts during merge:
 ```bash

git merge <branch-name>
git add <resolved-file>
git commit
 ```
# Part 4: Remote Repositories
## Task 9: Remote Setup
- Add a remote repository:
 ```bash

git remote add origin https://github.com/your-username/repo.git
 ```
- Verify the remote:
 ```bash

git remote -v
 ```
## Task 10: Push and Pull
- Push changes:
 ```bash

git push -u origin main
 ```
- Pull changes:
 ```bash

git pull origin main
 ```
## Task 11: Cloning a Repository
- Clone a remote repository:
 ```bash

git clone https://github.com/your-username/repo.git
 ```
# Part 5: Advanced Git
## Task 12: Stashing Changes
- Save uncommitted changes:
 ```bash

git stash
  ```
- Apply stashed changes:
 ```bash

git stash apply
 ```
- Drop the stash:
 ```bash

git stash drop
 ```
## Task 13: Tagging Commits
- Tag the current commit:
 ```bash

git tag -a v1.0 -m "Version 1.0 release"
 ```
- Push the tag:
 ```bash

git push origin v1.0
 ```
## Task 14: Rewriting Commit History
- Use interactive rebase:
 ```bash

git rebase -i HEAD~3
 ```
- Replace pick with edit or squash as needed.
## Task 15: Cherry-Picking Commits
- Apply a specific commit to another branch:
 ```bash

git cherry-pick <commit-hash>
```
# Part 6: Collaboration
## Task 16: Forking and Pull Requests
- Fork a repository and clone it locally:
 ```bash

git clone https://github.com/your-username/forked-repo.git
```
- Create a branch, make changes, and push:
 ```bash

git checkout -b fix-typo
echo "Typo fixed" >> README.md
git add README.md
git commit -m "Fixed a typo"
git push origin fix-typo
```
- Open a pull request on GitHub.
## Task 17: Simulating Team Collaboration
- Simulate conflicts by modifying the same file in two branches.
- Practice resolving conflicts with teammates.
# Part 7: Ignoring Files
## Task 18: Using .gitignore
- Create a .gitignore file:
 ```bash

echo "node_modules/" > .gitignore
 ```
- Add and commit the .gitignore:
 ```bash

git add .gitignore
git commit -m "Added .gitignore"
 ```
- Verify ignored files:
 ```bash

git status
 ```

# Part 8: Automation and Cleanup
## Task 19: Cleaning the Repository
- Remove untracked files:
 ```bash

git clean -f
 ```
## Task 20: Aliases and Shortcuts
- Create aliases:
 ```bash

git config --global alias.st status
git config --global alias.cm commit
```
- Use the aliases:
 ```bash

git st
git cm -m "Message"
```



=======
name
>>>>>>> feature-enhanced
