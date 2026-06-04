# Git Flow Basics Guide

Git Flow is a structured branching model for Git that helps teams manage software development and release cycles in an organized way. 

## 🌟 The Core Branches
There are two main, long-running branches:
* **`main` (or `master`)**: Stores the official release history. Every commit here is a production-ready version.
* **`develop`**: Serves as the integration branch for features. This is where the latest delivered changes for the next release live.

## 🛠️ The Supporting Branches
These are short-lived branches designed to handle specific tasks:
* **`feature/*`**: Used to develop new features for upcoming releases. They branch off `develop` and merge back into `develop`.
* **`release/*`**: Created when preparing a new production release. They allow for minor bug fixes and release meta-data preparation. They merge into both `develop` and `main`.
* **`hotfix/*`**: Created to quickly patch a critical bug in production. They branch off `main` and merge back into both `main` and `develop`.

---

## 💻 Standard Git Flow Commands

# Git Basics Introduction

Git is a distributed version control system used to track changes in source code.

## Getting Started
1. **Initialize** a repository: `git init`
2. **Clone** an existing project: `git clone <url>`

## Standard Workflow
To save changes, follow these steps:
* Check status: `git status`
* Stage files: `git add .`
* Commit: `git commit -m "Initial commit"`

## Syncing with GitHub
* Send changes: `git push origin main`
* Get updates: `git pull origin main`
