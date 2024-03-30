## Deploy to GitHub Pages:

### 1. Run this from terminal to install required package for gh-pages deployment

```
npm install gh-pages --save-dev
```

### 2. Add the below to pachage.json file

```
"homepage": "http://ismailchbiki.github.io/react-app",
.
.
.
scripts {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build"
}
```

### 3. After committing all changes to Git, run the below command from terminal

```
npm run deploy
```