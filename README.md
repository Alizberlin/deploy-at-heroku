1. Create a new React App and have your acc at Heroku -- cd into your project
2. Make sure you have node-modules and package json in your project
3. Check the versions of your Node and NPM with '$ node -v and npm -v' respectively 
4. Goto Json file, before dependencies write versions like below (outside dependencies or scripts)
```js
"engines": {
    "node": "16.0.0",
    "npm": "8.3.0"
},

```
5. run '$ npm run build'
if your are on windows or Mac go there 'https://devcenter.heroku.com/articles/heroku-cli#download-and-install '
6. run "$ heroku --version" if there is no version the "sudo snap install --classic heroku"
7. run  '$ heroku login'
8. when you are successfully logged-in run '$ heroku create app-name-of-ur-choice', 
if successful it will give you two links
one for your github: https://git.heroku.com/test-app.git
second URL to your app: https://test-app.herokuapp.com/
9. run '$ git init'.
10. then run '$ git remote add heroku and the github link that you got after step 7,
e.g "git remote add heroku https://git.heroku.com/test-app-react2626.git".
11. run '$ git remote -v'
you will get something like this
        heroku	https://test-app.herokuapp.com/ (fetch)
        heroku	https://test-app.herokuapp.com/ (push)
12. "$ git add . && git commit -m 'message'"
13. and at last run "$ git push heroku master"

if you make changes to your project
run 
```
 "$ npm run build"
 "$ git add . && git commit -m 'message'"
 "$ git push heroku master"
