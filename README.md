# Improved-Development-Workflow-and-Debugging

NPM is the package manager for JS and the world's largest software registry.

for custom scripts you have to use npm run

for reserved words like start you only have to do npm start

npm init creates a package with general info about your project

we can also install 3rd party packages

npm i <package_name>

npm install <package_name>

npm i <package_name> --save-dev puts in dev dependencies (packages used only by dev for better experience)

npm i <package_name> --save adds to dependencies, to be used by app to run certain things

npm i <package_name> -g is global package that can be used anywhere

## Core Node Packages:

- express
- body-parser

Note: When working and doing changes we would have to stop server and then run it again which is a pain, what we can do is install a third party package that does just that

npm i nodemon --save-dev (by default we get latest version)

We did --save-dev because it is only used for development and not production

go to package.json and add start script, set it to nodemon app.js
