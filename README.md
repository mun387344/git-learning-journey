#  Git & GitHub Hands-on Mastery

[![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)](https://git-scm.com/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/)
[![Version Control](https://img.shields.io/badge/Workflow-Trunk%20%26%20Feature%20Branch-blue?style=for-the-badge)]()
[![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)]()

---

##  Overview

This repository serves as a practical, hands-on workbench documenting foundational and intermediate **Git & GitHub** workflows. 

Rather than relying purely on theoretical tutorials, every command, branch transition, and merge strategy in this repository was executed locally and synchronized remotely to understand Git's underlying object graph, staging mechanics, and conflict resolution models.

---

##  Core Competencies & Command Reference

| Category | Commands | Practical Application |
| :--- | :--- | :--- |
| **Setup & Config** | `git init`, `git config`, `git clone` | Initializing workspaces, configuring user metadata, and cloning remote repos. |
| **Inspection & Staging** | `git status`, `git diff`, `git add` | Tracking working tree changes and selectively staging atomic modifications. |
| **Commit History** | `git commit -m`, `git log --oneline` | Writing semantic commit messages and reviewing linear commit logs. |
| **Branch Management** | `git branch`, `git checkout -b`, `git switch` | Isolating features and managing context switches across branches. |
| **Integration & Merging** | `git merge`, `git rebase` | Consolidating work streams and resolving manual merge conflicts cleanly. |
| **Undoing & Recovery** | `git reset`, `git revert`, `git restore`, `git stash` | Safe rollbacks, un-staging files, discarding working changes, and stashing states. |
| **Remote Sync** | `git remote`, `git push`, `git pull`, `git fetch` | Synchronizing local commits with GitHub and pulling upstream changes. |

---

##  Branching Strategy & Simulation

To simulate real-world collaborative engineering workflows, this repository incorporates multi-branch development models:

```text
main (production-ready)
 │
 ├── staging (integration & pre-release testing)
 │    │
 │    └── development (active working baseline)
 │         │
 │         └── feature/update-notes (isolated task branch)ractice.
```
Key Workflows Tested:
Feature Isolation: Building new files inside dedicated topic branches without polluting main.

Conflict Resolution: Intentionally producing divergent commit histories on identical lines, analyzing Git conflict markers (<<<<<<<, =======, >>>>>>>), and finalizing resolution commits.

Non-destructive Undo: Using git revert to roll back public histories without rewriting shared state.

 Practical Insights
Atomic Commits: Small, well-scoped commits with imperative messages simplify debugging and history traversals (git bisect / git log).

Stash Over Loss: Utilizing git stash prevents unfinished work from being accidentally wiped during branch switches.

The Index Layer: Understanding the deliberate boundary between the Working Directory, Staging Area (Index), and Repository (Commit Object) eliminates mistakes during complex merges.

 Author
Muna Mohammed

Aspiring Data & Software Professional
