# React-Git Project Deployment to GitHub Pages

## Steps to Deploy

### 1. Navigate to Your React Project Directory

cd react-git

### 2. Install gh-pages

Install the gh-pages package to help deploy your app:

npm install --save-dev gh-pages

### 3. Update package.json

"homepage": "https://haswanthakula.github.io/react-hosting"

Add predeploy and deploy scripts under the scripts section:

"scripts": {
  "start": "react-scripts start",
  "build": "react-scripts build",
  "test": "react-scripts test",
  "eject": "react-scripts eject",
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}

### 4. Link to the GitHub Repository

git remote add origin https://github.com/haswanthakula/react-hosting.git

### 5. Init,Add,Commit,Branch Your Changes

git init
git add .
git commit -m "Add deploy script and homepage URL"
git branch -M main
git push -u origin main

### 6. Deploy the App

npm run deploy

### 7. Access Your Deployed App

Your app will be live at: "Gitpages"










