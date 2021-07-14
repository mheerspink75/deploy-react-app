### deploy-react-app

*A guide to deploying create-react-app to GitHub Pages*

---

**1.** Install gh-pages npm package

```bash
npm i gh-pages
```

**2.** Create a new git repository branch and name it gh-pages


**3.** Update package,json with "homepage", "predeploy" and "deploy" scripts

```bash
},
"homepage": "https://mheerspink75.github.io/deploy-react-app/",
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build",
  "start": "react-scripts start",
  "build": "react-scripts build",
  "test": "react-scripts test",
  "eject": "react-scripts eject"
},
```
  
**4.** Run npm predeploy script

```bash
npm run predeploy
```

**5.** Run npm deploy script

```bash
npm run deploy
```

**6.** Check the gh-pages branch of the git repository to view the production files

**7.** Visit the homepage url: https://mheerspink75.github.io/deploy-react-app/