# React JS Crash Course - 2019
This repo will go through travery media's React tutorial updated for 2019. This tutorial uses mainly classed based `React.Component`s. It includes themes such as;
- Creating new class based `React.Component`s
- Rendering React Components
- Passing props between `React.Component`s
- Passing functions between `React.Component`s
- Conditionally setting className and style with functions
- Altering the state from 'down the tree' (without the Context API)
- Handling form events 
- Using `React.Fragment`s
- Updating state with `setState` (deleting, inserting and updating *todos*)
- `Route` and `BrowserRouter` from `react-router-dom`

### Available Scripts

In the project directory, you can run:

##### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

##### `npm test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

##### `npm run build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

# Deploy Process (Github Pages)
**Install gh-pages**
```sh
npm install gh-pages --save-dev
```
**Edit `package.json`**
```
# Add the homepage
"homepage": "https://danielc92.github.io/react-tutorial-traversy"
# Add predeploy and deploy to scripts
"scripts": {
"start": "react-scripts start",
"predeploy": "npm run build",
"deploy": "gh-pages -d build",
...
```
**Make sure router is correct
Change any `BrowserRouter` to `HashRouter` in main `App.js`

**Deploy**
```sh
# This will build and deploy to a new branch called gh-pages
# Modify the hosting source in settings from master branch to gh-pages
npm run deploy
```

# Sources
- [React JS Crash Course - 2019](https://www.youtube.com/watch?v=sBws8MSXN7A)
- [Deploy React to gh-pages Guide](https://www.youtube.com/watch?v=4NapRkCazks)