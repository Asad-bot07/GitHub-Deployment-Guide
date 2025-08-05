# 📘 GitHub Pages Deployment Guide

Welcome! This document will walk you through deploying your project to **GitHub Pages**, one of the easiest ways to host static websites directly from a GitHub repository.

We’ll cover two types of deployments:

- **Chapter 1:** Deploying a Basic Static Project (HTML/CSS/JS)
- **Chapter 2:** Deploying a React App (using `gh-pages`)

---

## 📖 Chapter 1: Deploying a Static Website (HTML, CSS, JS)

### 🧠 What You Need to Know
GitHub Pages allows you to host static websites (no backend) straight from a GitHub repository. If your project has an `index.html` file, you’re good to go.

### 🔧 Requirements
- A GitHub account
- Git installed on your computer
- A folder containing your website files (like `index.html`, `style.css`, `script.js`)

---

### 🪜 Step-by-Step Instructions

#### Step 1: Initialize Git
Open your terminal or command prompt, navigate to your project folder, and run:
```bash
git init
git add .
git commit -m "Initial commit"
```
#### Step 2: Create a GitHub Repository

- Go to [GitHub](https://github.com)
- Click the + icon (top right) → New repository
- Name your repository (e.g., my-portfolio)
- Do not initialize with README or .gitignore

#### Step 3: Connect Your Local Repo to GitHub
Replace the URL below with your own:

```
git remote add origin https://github.com/your-username/your-repo-name.git
git branch -M main
git push -u origin main
```

#### Step 4: Enable GitHub Pages

- Open your repository on GitHub
- Click Settings
- Scroll to Pages
- Under Source, select main branch and /root
- Click Save

#### ✅ Done!
Your site will be published at:
```
https://your-username.github.io/your-repo-name
```
<<<<<<< HEAD:StaticDeploy.md
---
=======
>>>>>>> 5f6e5339734d6152e287819eb682fcea45e750f1:Guide.md
