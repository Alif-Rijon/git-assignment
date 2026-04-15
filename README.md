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
