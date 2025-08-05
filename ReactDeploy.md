# ⚛️ Chapter 2: Deploying a React App (create-react-app)

#### 🧠 Why Is This Different?
React apps are built using `JSX` and modern JavaScript. Before deployment, React needs to compile everything into plain HTML, CSS, and JS using a build process.
## 🔧 Requirements

- React app created using create-react-app(can be used with Vite too)
- A GitHub account
- Node.js installed (npm should be available)

### 🪜 Step-by-Step Instructions

#### Step 1: Install gh-pages

This package helps you deploy the build folder to GitHub Pages.

```
npm install gh-pages --save-dev
```
#### Step 2: Configure package.json

- Add the homepage field at the top:

```
"homepage": "https://your-username.github.io/your-repo-name",
```
- Update your scripts section:
```
"scripts": {
  "start": "react-scripts start",
  "build": "react-scripts build",
  "predeploy": "npm run build",
  "deploy": "gh-pages -d dist"
}
```

#### Step 3: Initialize Git and Push Code
```
git init
git remote add origin https://github.com/your-username/your-repo-name.git
git add .
git commit -m "Initial React commit"
git branch -M main
git push -u origin main
```
#### Step 4: Deploy!
Now run the deploy command:
```
npm run build
npm run deploy
```
##### This will:
- Build your project (npm run build)
- Push the contents of the build/ folder to a special gh-pages branch

✅ Done!
Your React app will be live at:
```
https://your-username.github.io/your-repo-name
```

### 🧠 Tips & Common Issues

#### React Router Issues?
If you're using `React Router`, GitHub Pages may show a 404 on page refresh.
- Add this to public/index.html:
```
<base href="/" />
```

- Or use a HashRouter instead of BrowserRouter in your React app:
```
import { HashRouter } from "react-router-dom";
```
