---
title: Doing magic with Git
date: 15 December 2023
description: since git does not give us breathing space, i should write about it. ki okan gbogbo wa ma bale...
keywords: github, product, gitlab, git
draft: false
---

i'm here again. this time, i want you to know that Git is a powerful version control system that helps developers manage their code efficiently. even if you're an OP  programmer or just starting out coding, understanding Git is crucial for collaborative and organized development. i would  explore the basics of Git and how it can change your workflow in this post.

## so, what is Git?

according to google, Git is a distributed version control system, designed to track changes in source code during software development. Created by Linus Torvalds in 2005, Git has become the industry standard for version control due to its flexibility and speed.

## let's talk about the key concepts

### Repository

At the core of Git is the repository, or "repo" for short. A repo is a directory that contains your project's files and the entire history of changes made. You can have a local repository on your machine and a remote repository on a server.

### Commit

A commit is a snapshot of your project at a specific point in time. if you were playing gta, this is like saving your game. Each commit can have a unique identifier to make it easy to track changes and revert to previous states.

### Branch

Branches allow you to work on different features or bug fixes simultaneously. The main branch is usually called "master" (i like mine as main tho), and you can create new branches for specific tasks. Once your changes are tested and ready, they can be merged back into the main branch.

## Basic Git Workflow (for new lads)

1. **Initialize a Repository:**
   To start using Git, navigate to your project directory in the terminal and run `git init`. This creates a new Git repository.

2. **Stage Changes:**
   Use `git add` to stage changes for the next commit. You can either stage specific files or all changes. You can either use `git add .` or `git add filename` cause it depends if you want to add all changes or a specific file change.

3. **Commit Changes:**
   Commit your changes using `git commit -m "put whatever you want to say here"`. This saves a snapshot of your project.

4. **Create Branches:**
   Utilize branches for different tasks. Create a new branch with `git branch branch_name` and switch to it with `git checkout branch_name`. More like `git branch master` or similar.

5. **Merge Changes:**
   Once your changes are tested and ready, merge them back into the main branch using `git merge branch_name`.

6. **Push and Pull:**
   If you're working in a team, use `git push` to upload your changes to the remote repository. To fetch changes from the remote, use `git pull`.

## Collaboration with Git

Git allows seamless collaboration between devs, cause services like GitHub, GitLab, or even Bitbucket allow teams to host their repositories, track issues, and manage pull requests too. These platforms make it easy for multiple developers to contribute to a project without conflicts. That's the sleekest part of git. ❤️
