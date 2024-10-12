---
title: Git and Github
draft: false
tags:
  - git
  - github
  - version-control
---
# Git Basics: A Step-by-Step Guide

  

This guide walks you through Git, its commands, and how everything works step by step. Git is a distributed version control system used to track changes in code, collaborate with others, and manage different versions of a project.

  

---

## Step 1: Setting Up Git in a Folder

  

### 1.1. Open Command Prompt/Terminal in Folder

  

To open the terminal in your folder:

  

1. Create a folder where you want to initialize a Git repository.

2. Navigate to that folder in your File Explorer (Windows) or Finder (Mac).

3. In the folder's address bar (Windows), type `cmd` and press Enter to open Command Prompt in the folder. On Mac/Linux, right-click and open the terminal.

  

## Step 2: Initialize a Git Repository

  

### 2.1. git init

  

Once your terminal is open, type `git init`. This command initializes an empty Git repository in your folder. It creates a `.git` folder that contains all the internal data Git uses for version control.

  

## Step 3: Local Area, Staging Area, and Commit

  

### 3.1. Working Directory (Local Area)

The working directory is where your project files are. When you create, modify, or delete files, these changes occur in the working directory. Git doesn’t automatically track these changes.

  

### 3.2. Staging Area

When you’re ready to tell Git to track specific changes, you add files to the staging area using `git add <filename>`. The staging area is where you prepare files for a commit.

  

### 3.3. Commit

After staging your files, use `git commit -m "message"` to permanently store the changes. A commit is a snapshot of your project at a specific point in time.

  

#### Commands:

- `git add <filename>`: Stages specific files.

- `git add .`: Stages all modified files in the current directory.

- `git commit -m "message"`: Commits staged changes with a message.

  

## Step 4: Checking Git Status

  

### 4.1. git status

This command shows the current state of your working directory and staging area. It tells you which files are modified, staged, or committed.

  

## Step 5: Branching and Why It's Important

  

### 5.1. Branches

A branch is a separate version of your project. By default, Git starts on the main branch (previously called master). You can create new branches to work on features or bug fixes without affecting the main branch.

  

#### Commands:

- `git branch`: Shows the current branch.

- `git branch <branch-name>`: Creates a new branch.

- `git checkout <branch-name>`: Switches to another branch.

  

### 5.2. Why Branches Are Important

Branches allow you to experiment and make changes without breaking the main project. You can merge branches back into the main project once your work is done.

  

## Step 6: Merging Branches

  

### 6.1. Merging

When you're done with work on a branch, merge it back into the main branch (or any other branch) using `git merge <branch-name>`.

  

### 6.2. Merge Conflicts

Sometimes merging branches may lead to merge conflicts, where changes in different branches contradict each other. Git pauses the merge and asks you to resolve the conflicts.

  

#### Resolving a Conflict:

1. Git will mark the conflicting areas in the affected files.

2. Open the files, find the conflicts, and decide which version to keep.

3. After resolving conflicts, stage the file (`git add <filename>`) and commit it (`git commit`).

  

## Step 7: Collaborating on GitHub

  

### 7.1. GitHub Setup

GitHub is a cloud service for hosting Git repositories, allowing for remote collaboration.

  

#### Commands:

- `git remote add origin <repo-url>`: Links your local repository to a remote GitHub repository.

- `git push origin <branch-name>`: Pushes your local commits to the remote GitHub repository.

  

### 7.2. Pull Requests

On GitHub, you can create pull requests to propose changes. Other team members can review and discuss changes before merging them into the main project.

  

## Step 8: VSCode Git Integration

  

### 8.1. Git Built into VSCode

VSCode comes with built-in Git support, making it easier to manage repositories.

  

#### Key Features:

- *Source Control Tab*: Shows your current changes and branches.

- *Commit Button*: Allows you to commit directly from VSCode.

- *Branch Switcher*: Easily switch between branches.

- *Merge Tools*: Built-in merge conflict resolution.

  

## Additional Topics: .gitignore

  

### 9.1. .gitignore

The `.gitignore` file tells Git which files or directories to ignore. This is useful for excluding things like build files or sensitive data from your repository.

  

---

  

By following this guide, you will have a solid foundation for using Git and GitHub effectively to manage your projects.