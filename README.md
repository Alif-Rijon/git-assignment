# 📘 Advanced Git Workflow & Version Control Assignment

## 🎯 Objective
This project demonstrates advanced Git concepts including:
- Branching strategy
- Merge vs Rebase
- Commit history management (Squash & Reword)
- Real-world Git workflow simulation

---

## 🧠 Branch Structure

The following branches were used in this project:

- main
- develop
- feature/login
- feature/payment
- feature/profile
- bugfix/login-error

---

## ⚙️ Workflow Summary

### 1. Branching Strategy
A structured Git workflow was followed:

- `main` → Production-ready code
- `develop` → Integration branch
- `feature/*` → New features development
- `bugfix/*` → Bug fixing branch

---

### 2. Feature Development

#### Feature/Login
- Implemented login functionality step by step
- Multiple commits were created
- Later optimized using squash and reword

#### Feature/Payment
- Payment feature implemented
- Merged into develop using fast-forward merge

#### Feature/Profile
- Profile feature implemented
- Integrated using rebase strategy for clean history

---

### 3. Merge Strategy

#### Fast-forward Merge
Used for simple integration:

- feature/payment → develop

#### No Fast-forward Merge
Used to preserve branch history:

```bash
git merge --no-ff feature/login
```
## Commands Used

git init  
git branch  
git checkout -b develop  
git checkout -b feature/login  
git checkout -b feature/payment  
git checkout -b feature/profile  
git checkout -b bugfix/login-error  

git merge  
git merge --no-ff feature/login  
git rebase develop  
git rebase -i HEAD~5  

git log --oneline --graph --all  
git push --all origin

## Screenshots

### Branching
![Branches](images/branch.png)

### Commit History
![Commits](images/graph.png)

### Pull Request / Repository View
![Repo](images/repo.png)

## Merge vs Rebase

### Merge
- Combines branches using a merge commit
- Preserves full history
- Used for team collaboration

### Rebase
- Rewrites commit history
- Creates linear history
- Used for clean project structure

## Squash vs Reword

### Squash
- Combines multiple commits into one
- Used to clean commit history

### Reword
- Changes commit message
- Used to improve readability and clarity
