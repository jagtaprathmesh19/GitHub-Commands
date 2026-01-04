
# 🚀 GitHub Commands — Practical Guide

### Project Scenario: **ShopStream**

> **ShopStream** is a collaborative e-commerce web application.
> This guide walks through the **entire Git lifecycle** — from setup ➜ feature development ➜ collaboration ➜ release ➜ debugging.

---

## 🧩 How to Read This Guide

Each command follows this pattern:

> **Command**
> **Use Case (ShopStream example)**
> *What the command actually does*

---

## 🔹 Phase 1: Project Setup & Configuration

### Initialize & Connect Repositories

```bash
git init
```

**Start the ShopStream project from scratch**
*Initializes a new Git repository in the current folder.*

---

```bash
git config
```

**Set your developer identity for ShopStream commits**
*Configures username, email, and preferences (local or global).*

---

```bash
git clone [url]
```

**Download the ShopStream repository to a new machine**
*Copies the entire remote repository including history and branches.*

---

```bash
git remote add [name] [url]
```

**Connect your local ShopStream repo to GitHub**
*Allows pushing and pulling code from a remote server.*

---

## 🔹 Phase 2: Feature Development

### (Example: Shopping Cart)

### Branching & Development

```bash
git branch [name]
```

**Create a feature branch (`shopping-cart`)**
*Creates an isolated workspace for new features.*

---

```bash
git checkout [name]
```

**Switch to the shopping-cart branch**
*Updates your working directory to that branch.*

---

```bash
git switch [name]
```

**Safely switch branches (modern method)**
*A clearer alternative to `checkout` for branch switching.*

---

### Tracking Changes

```bash
git status
```

**Check modified cart files**
*Shows staged, unstaged, and untracked files.*

---

```bash
git diff
```

**Review code changes before saving**
*Displays line-by-line differences.*

---

```bash
git add [file]
```

**Stage `Cart.js` for commit**
*Moves changes to the staging area.*

---

```bash
git commit -m "message"
```

**Save shopping cart logic to history**
*Creates a snapshot of staged changes.*

---

```bash
git restore [file]
```

**Discard broken experimental changes**
*Reverts files back to last committed state.*

---

## 🔹 Phase 3: Collaboration & Sync

```bash
git fetch
```

**Check teammate updates without merging**
*Downloads remote changes only.*

---

```bash
git pull
```

**Update your branch with team changes**
*Fetches and merges in one step.*

---

```bash
git push
```

**Upload your shopping-cart feature to GitHub**
*Publishes local commits to remote.*

---

```bash
git stash
```

**Pause feature work to fix an urgent bug**
*Saves uncommitted changes temporarily.*

---

```bash
git stash pop
```

**Resume paused work**
*Restores the latest stash.*

---

## 🔹 Phase 4: Inspecting History

```bash
git log
```

**View ShopStream commit history**
*Shows commits, authors, dates, and messages.*

---

```bash
git show [commit]
```

**Inspect a specific commit**
*Displays exact code changes.*

---

```bash
git blame [file]
```

**Find who wrote a problematic line**
*Shows author and commit per line.*

---

```bash
git shortlog
```

**See contribution summary per developer**
*Groups commits by author.*

---

## 🔹 Phase 5: Integration & Release

```bash
git merge [branch]
```

**Merge shopping-cart into main**
*Combines branch histories.*

---

```bash
git rebase [branch]
```

**Update feature branch with latest main code**
*Rewrites commits for clean linear history.*

---

```bash
git tag [name]
```

**Mark ShopStream v1.0 release**
*Creates a version reference.*

---

## 🔹 Phase 6: Undo, Fixes & Debugging

```bash
git reset --soft [commit]
```

**Undo commit but keep changes**
*Moves HEAD while preserving staged code.*

---

```bash
git reset --hard [commit]
```

**Fully revert to a safe state**
*Deletes all local changes.*

---

```bash
git revert [commit]
```

**Safely undo a production bug**
*Creates a new commit that cancels an old one.*

---

```bash
git cherry-pick [commit]
```

**Apply a specific fix to another branch**
*Copies a single commit.*

---

```bash
git bisect
```

**Find the exact commit that caused a bug**
*Uses binary search to isolate failures.*

---

# ⚙️ Essential Git Flags (Quick Reference)

## 🔹 Setup & Configuration

```bash
git config --global
```

*Applies settings to all repositories.*

```bash
git clone --depth 1
```

*Shallow clone (latest commit only).*

```bash
git remote -v
```

*Shows remote URLs.*

---

## 🔹 Feature Development

```bash
git checkout -b feature
```

*Create + switch branch.*

```bash
git status -s
```

*Short status output.*

```bash
git add -p
```

*Stage selected code chunks.*

```bash
git commit -a
```

*Auto-stage modified files.*

```bash
git commit --amend
```

*Edit last commit.*

---

## 🔹 Collaboration

```bash
git fetch --prune
```

*Remove deleted remote branches.*

```bash
git pull --rebase
```

*Replay commits cleanly.*

```bash
git push -u
```

*Set upstream branch.*

```bash
git push --force
```

*Overwrite remote history (use carefully).*

```bash
git stash -u
```

*Stash tracked + untracked files.*

---

## 🔹 History & Cleanup

```bash
git log --oneline --graph
```

*Compact visual history.*

```bash
git blame -L 10,20 file
```

*Blame specific lines.*

```bash
git clean -n
```

*Preview cleanup.*

```bash
git clean -fd
```

*Delete untracked files & folders.*

```bash
git reflog
```

*Recover lost commits or branches.*

---


