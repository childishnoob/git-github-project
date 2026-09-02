# Git & GitHub Workflow Project

## Description

This project demonstrates the basic Git and GitHub workflow used for version control and collaborative development.

It covers repository creation, commits, branches, merging, merge conflict resolution, remote repositories, pushing and pulling changes, and GitHub Pull Requests.

## Features

- Initializes a Git repository.
- Tracks files using Git.
- Stages and commits changes.
- Uses a `.gitignore` file.
- Creates and switches between branches.
- Uses feature branches for independent development.
- Merges branches into `main`.
- Creates and resolves merge conflicts.
- Connects a local repository to GitHub.
- Pushes changes and branches to GitHub.
- Pulls changes from GitHub.
- Creates and merges GitHub Pull Requests.
- Manages local and remote branches.
- Views Git commit history.

## Requirements

- Git
- GitHub account
- GitHub CLI (`gh`) for authentication
- Linux or another Unix-like environment

## Usage

Initialize a repository:

    git init

Check the repository status:

    git status

Stage files:

    git add <file>

Commit changes:

    git commit -m "Commit message"

Create and switch to a feature branch:

    git switch -c feature/branch-name

Merge a feature branch:

    git switch main
    git merge feature/branch-name

Connect the local repository to GitHub:

    git remote add origin <github-repository-url>

Push the main branch:

    git push -u origin main

Pull changes from GitHub:

    git pull

## Git Workflow

The workflow practiced in this project was:

1. Created a local project directory.
2. Initialized a Git repository.
3. Created project files.
4. Added files to the staging area.
5. Created the initial commit.
6. Added a `.gitignore` file.
7. Created and switched between feature branches.
8. Made changes on feature branches.
9. Committed feature changes.
10. Merged feature branches into `main`.
11. Created a merge conflict by modifying the same line differently on two branches.
12. Resolved the merge conflict manually.
13. Committed the conflict resolution.
14. Created a GitHub repository.
15. Connected the local repository to GitHub using a remote named `origin`.
16. Pushed the local repository to GitHub.
17. Created a feature branch for the Pull Request workflow.
18. Pushed the feature branch to GitHub.
19. Created a Pull Request from the feature branch into `main`.
20. Merged the Pull Request on GitHub.
21. Used `git pull` to synchronize the local repository with GitHub.
22. Deleted merged local and remote branches.
23. Verified the final repository state.

## Branching

The project used feature branches to keep changes separate from the stable `main` branch.

Example:

    main
      |
      |------ feature/update-notes
      |
      |------ feature/conflict-test
      |
      |------ feature/github-pr

After completing the work, the changes were merged back into `main`.

## Merge Conflict

A merge conflict was deliberately created by changing the same line differently on two branches.

Git marked the conflicting section using:

    <<<<<<< HEAD
    =======
    >>>>>>> branch-name

The conflict was resolved by manually selecting the desired content, staging the file, and committing the merge result.

## Pull Request

A GitHub Pull Request was created from:

    feature/github-pr

into:

    main

The Pull Request was successfully merged on GitHub.

## Useful Commands

    git init
    git status
    git add
    git commit
    git branch
    git switch
    git merge
    git log
    git diff
    git remote -v
    git push
    git pull
    git fetch

## Testing

The Git workflow was tested with:

- Repository initialization
- File staging
- Multiple commits
- Feature branch creation
- Branch switching
- Branch merging
- Merge conflict creation
- Merge conflict resolution
- Remote repository connection
- Pushing to GitHub
- Pulling changes from GitHub
- GitHub Pull Request creation
- Pull Request merging
- Local and remote branch deletion
- Final repository status verification

## Result

The project successfully demonstrates a complete basic Git and GitHub workflow, including version control, branching, merging, conflict resolution, remote repositories, GitHub Pull Requests, and repository synchronization.
