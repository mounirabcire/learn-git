# ✨ Learn Advanced Git ✨

In this repository, I explored advanced Git techniques essential for real-world team collaboration, following along with [this YouTube video](https://youtu.be/S7XpTAnSDL4?si=2JOhyg6P7g18_3dh) by **JavaScript Mastery**.

## 📊 What I Knew About Git Before

### ℹ️ Terms

- **Git**: A version control system that helps track changes in files, manage project versions, and collaborate with others.
- **GitHub**: A cloud platform that allows storing your Git repositories online and collaborating with others.
- **Repository**: A project folder where Git tracks everything within it.
- **Commit Messages**: Should be written in the imperative mood to describe what the code will do after applying the changes.

### ⚙️ Commands

- `git init`: Creates a new Git repository in a project folder by creating a hidden `.git` folder that handles everything, including remote repos, commit history, branches, and more.
- `git config --global user.name` / `git config --global user.email`: Configures user settings to display information when committing changes.
- `git status`: Checks the current status of the repository.
- `git add .` / `git add file-name`: Moves the changed files to the staging area.
- `git commit -m "commit message"`: Saves the staged changes with a meaningful commit message.
- `git log`: Displays the commit history.
- `git remote add origin <github-remote-link>`: Links your local repository to a remote repository.
- `git push -u origin main`: Pushes the local `main` branch to the remote `origin` branch.

## ✨ What I Learned 

### 📖 Terms

- **Head**: A pointer to the latest commit. If you run `git checkout <commit-id>`, the head will enter a detached state, meaning it no longer points to the latest commit.
- **Repository Types**:
  - **Local Repository**: A version of the project stored on your local machine (private).
  - **Remote Repository**: A version of the project stored on a server, used for sharing code and collaboration.
- **Origin**: The default name Git assigns to a remote repository (e.g., `origin = github.com/jsm/portfolio`).
- **Branches**: Allow creating copies of your project at a specific point in time, enabling changes in the copied version without affecting the original. **Merging** combines these changes back into the original version.
- **Commit Messages**: Should answer the question: *If applied to the code base, this commit will...*
- **Pull Request (PR)**: A proposal to merge specific changes from a branch into the default branch (e.g., `main`). It allows for team review and feedback before merging.
- **Merge Conflicts**: Occur when two or more developers modify the same file at the same lines. Git gets confused, requiring manual conflict resolution.
- How to resolve simple merge conflicts: Learn to handle merge conflicts by identifying conflicting changes in the file, editing the file to keep the desired changes, and then staging and committing the resolved version.
- How to use GUI (I didn’t really like this approach): Explored using a graphical user interface (GUI) for Git operations, but found it less intuitive compared to using the command line.

### ⚙️ Commands

- `git config --global init.defaultBranch <branch-name>`: Sets the default branch name for new repositories.
- `git checkout <branch-name>` / `git checkout <commit-id>`: Switches between branches or checks the state of the repository at a specific commit.
- `-u` flag: Sets an upstream branch to simplify future pushes or pulls by automatically linking the remote repository to the local branch.
- `git branch`: Lists all local branches.
- `git branch -r`: Lists all remote branches.
- `git branch <branch-name>`: Creates a new branch.
- `git checkout -b <branch-name>`: Creates a new branch and immediately switches to it.
- `git branch <branch-name> <source-branch>`: Creates a new branch based on a specified source branch.
- `git pull <remote> <branch>`: Fetches and integrates changes from a remote repository into the local branch.
- `git merge <branch-name>`: Merges code from a specified branch into the current branch.
- `git branch -d <branch-name>`: Deletes a local branch if it has been merged (safe delete). Use `-D` for forced deletion.
- `git push origin --delete <branch-name>`: Deletes a remote branch.
- `git reset --soft <commit-id>`: Resets the repository to a specific commit but keeps the changes staged.
- `git reset --hard <commit-id>`: Resets the repository to a specific commit and discards all changes.
- `git reset <commit-id>`: Resets to a specific commit without staging or discarding changes.
- `git revert <commit-id>`: Creates a new commit that undoes changes from a specific commit.
- `git stash`: Temporarily saves changes not ready to commit.
- `git stash apply <stash-name>`: Applies a specific stash.
- `git stash list`: Lists all stashes.
- `git stash save "custom message"`: Saves a stash with a custom message.
