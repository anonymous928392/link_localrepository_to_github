# 🧭 Git & GitHub Linking Guide

This guide explains how to **connect a local repository to GitHub**, either by creating a new repo or linking an existing one.

---

## 🧩 Option 1 — Create a New GitHub Repository (from Local Folder)

If you already have a local project and want to create a **new repository** on GitHub:

### 1. Initialize Git in your local folder
```bash
git init
```

### 2. Add your files
```bash
git add .
```

### 3. Commit them
```bash
git commit -m "Innitial commit"
```

### 4. Create a repository on Github 
If you have the GitHub CLI (gh) installed:

```bash
gh repo create my-repo-name --private --source=. --remote=origin 
```
or
```bash
gh repo create my-repo-name --public --source=. --remote=origin 
```



### 5. Push your local commits

```bash
git push -u origin main

```

## 🧩 Option 2 — Link to an Existing GitHub Repository

### 1. Initialize Git locally (if not already)
```bash
git init
```

### 2. Add a remote that points to GitHub
```bash
git remote add origin https://github.com/USERNAME/REPO_NAME.git
```

### 3. Add your files
```bash
git add .
```

### 4. Commit them
```bash
git commit -m "Initial commit"
```

### 5. Push your code to GitHub
```bash
git branch -M main
git push -u origin main
```

###  Verify Connection
```bash
git remote -v
```


##  Useful Commands
```bash
git branch
git pull origin main
git add .
git status
git commit -m "Update"
git push
```


