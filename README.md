## Deploy to GitHub Pages

### 1. Install the required package for gh-pages deployment

Run the following command in the terminal to install the necessary package:

```bash
npm install gh-pages --save-dev
```

### 2. Configure "package.json"

Add the following lines to the `package.json` file:

```bash
{
  "homepage": "http://ismailchbiki.github.io/react-app",
  .
  .
  .
  "scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build"
  }
}
```

### 3. Deploy Your App
After pushing all changes to Git, run the following command from the terminal:<br>
The command will build the project and deploy it to GitHub Pages.

```bash
npm run deploy
```