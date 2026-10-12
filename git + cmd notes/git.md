# Git Commands

---

### Workflow

```bash
git add .
git commit -m "message"
git push
```

---

### NOTE:

* `git init` = new repo; `git clone` = copy existing repo<br>
* `git commit` is local; `git push` uploads to remote<br>
* `origin` is just the default remote name<br>
* `git clone` already sets remote; no need for `git remote add origin` after it<br>
* use `git status` whenever unsure<br>
---

### Basic Setup

```bash
git config --global user.name "your name"
git config --global user.email "your@email.com"
```

Sets identity for commits<br>

---

### Repository Setup

```bash
git init
```

Create a new empty local repository<br>

```bash
git clone <url>
```

Clone an existing remote repository to your local machine (includes files, history, branches, and sets `origin` automatically)<br>

```bash
git remote add origin <link>
```

Manually connect local repo to a remote (used after `init`, not needed after `clone`)<br>

```bash
git remote -v
```

Show connected remotes<br>

---

### Branching

```bash
git branch
```

List branches<br>

```bash
git branch -M <name>
```

Rename current branch<br>

```bash
git checkout -b <name>
```

Create and switch to new branch<br>

```bash
git checkout <name>
```

Switch branch<br>

```bash
git branch -d <name>
```

Delete branch<br>

---

### Status & Logs

```bash
git status
```

Show current file states and suggested actions<br>

```bash
git log
```

Show commit history<br>

```bash
git log --oneline
```

Compact history view<br>

---

### Staging

```bash
git add <file>
```

Stage specific file<br>

```bash
git add .
```

Stage all changes<br>

---

### Commits

```bash
git commit -m "message"
```

Save a snapshot of staged changes to local history (does NOT push to GitHub)<br>

---

### Remote (GitHub)

```bash
git push origin main
```

Upload commits to remote branch<br>

```bash
git push -u origin main
```

Upload and set upstream (so future `git push` works without args)<br>

```bash
git pull
```

Fetch + merge changes from remote<br>

```bash
git fetch
```

Download changes without merging<br>

---

### Viewing Changes

```bash
git diff
```

Show unstaged changes<br>

```bash
git diff --staged
```

Show staged changes<br>

---

### Undo / Fix

```bash
git restore <file>
```

Discard working directory changes<br>

```bash
git restore --staged <file>
```

Unstage file<br>

```bash
git reset HEAD~1
```

Remove last commit, keep changes<br>

```bash
git reset --hard HEAD~1
```

Remove last commit and changes permanently<br>

---

### Stash

```bash
git stash
```

Temporarily save uncommitted changes<br>

```bash
git stash pop
```

Restore stashed changes<br>

---

### File Operations

```bash
git rm <file>
```

Remove file and stage deletion<br>

```bash
git mv old.txt new.txt
```

Rename/move file<br>

---