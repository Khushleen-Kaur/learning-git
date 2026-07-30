# 🚀 Git & GitHub Workflow

A quick reference for the most commonly used Git commands.

---

## 🆕 1. Initialize Git Repository

```bash
git init
```

Initializes Git in your project folder.

---

## 📂 2. Check Repository Status

```bash
git status
```

Shows modified, staged, and untracked files.

---

## ➕ 3. Stage Files

### Stage all files

```bash
git add .
```

### Stage a specific file

```bash
git add filename
```

---

## 💾 4. Commit Changes

```bash
git commit -m "Your commit message"
```

Saves the staged changes.

Example:

```bash
git commit -m "Added login page"
```

---

## 🌿 5. Check Current Branch

```bash
git branch
```

---

## 🔄 6. Rename Branch to main (First Time)

```bash
git branch -M main
```

---

## 🔗 7. Connect Local Repository to GitHub

```bash
git remote add origin https://github.com/USERNAME/REPOSITORY.git
```

Check remote:

```bash
git remote -v
```

---

## ☁️ 8. Push Project to GitHub (First Time)

```bash
git push -u origin main
```

The `-u` flag sets the upstream branch, so next time you only need:

```bash
git push
```

---

# 🔄 Daily Workflow

Whenever you make changes:

### Check status

```bash
git status
```

### Stage changes

```bash
git add .
```

### Commit

```bash
git commit -m "Describe your changes"
```

### Push

```bash
git push
```

---

# 📥 Pull Latest Changes

Before starting work on another device or after collaborators push changes:

```bash
git pull origin main
```

Or simply:

```bash
git pull
```

---

# 📜 View Commit History

```bash
git log
```

Short version:

```bash
git log --oneline
```

---

# 📂 View Remote Repository

```bash
git remote -v
```

---

# 🗑️ Remove Remote Repository

```bash
git remote remove origin
```

---

# 🔄 Change Remote Repository URL

```bash
git remote set-url origin NEW_REPOSITORY_URL
```

---

# 🌱 Create a New Branch

```bash
git checkout -b feature-name
```

---

# 🔀 Switch Branch

```bash
git checkout branch-name
```

---

# 🔀 Merge Branch

Switch to main:

```bash
git checkout main
```

Merge:

```bash
git merge feature-name
```

---

# 🚫 Ignore Files

Create a `.gitignore` file.

Example:

```text
node_modules/
.env
dist/
```

---

# ❌ Unstage a File

```bash
git restore --staged filename
```

---

# ♻️ Discard Local Changes

```bash
git restore filename
```

Discard all changes:

```bash
git restore .
```

---

# 📌 Clone an Existing Repository

```bash
git clone https://github.com/USERNAME/REPOSITORY.git
```

---

# ⚡ Complete Git Workflow

```text
Create Project
      │
      ▼
git init
      │
      ▼
git status
      │
      ▼
git add .
      │
      ▼
git commit -m "Initial commit"
      │
      ▼
git branch -M main
      │
      ▼
git remote add origin <repo-url>
      │
      ▼
git push -u origin main
      │
      ▼
───────────────────────────────
Daily Workflow
───────────────────────────────
git status
      │
      ▼
git add .
      │
      ▼
git commit -m "Updated project"
      │
      ▼
git push
```

---

# ⭐ Most Used Commands

| Command | Purpose |
|---------|---------|
| `git init` | Initialize Git |
| `git status` | Check changes |
| `git add .` | Stage all files |
| `git commit -m "msg"` | Save changes |
| `git push` | Upload to GitHub |
| `git pull` | Download latest changes |
| `git clone URL` | Copy repository |
| `git branch` | List branches |
| `git checkout branch` | Switch branch |
| `git merge branch` | Merge branches |
| `git log --oneline` | View commits |
| `git remote -v` | View remote repository |

---

## 💡 Golden Rule

```text
Code
   ↓
git status
   ↓
git add .
   ↓
git commit -m "Meaningful message"
   ↓
git push
```

Repeat this workflow every time you make changes.