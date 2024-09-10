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

## Types of Errors:

1. Syntax Errors: Typo, forget () or {}

2. Runtime Errors: You execute code that breaks when it runs

3. Logical Errors: No Error Messages but the app doesn't work the way it should

## Finding & Fixing Syntax Err:

It will mark red in code editor and app crashes instantly on run

In case of typo it might be same line but in case of ) or } it will put red mark at end of block and not at place of missing/extra bracket or braces

## Finding & Fixing Runtime Err:

Code runs but it breaks at a certain point, you should read the error message since they are helpful, look at top of message and not bottom where the meaningful hints are

For e.g. we only work on res once and once it is sent we can't edit, so if we don't end process it will become a runtime error like changing header twice instead of once

## Logical Errors:

This is where there are no errors but the app doesn't do what we want. We are kinda at fault here...

For example using wrong index const message = parsedBody.explit('=')[0]; instead of [1] so we get key before = instead of value after =

We can go to Debug, Start Debugging, choose environment like Node.JS, an extra bar will pop up and console says debugger is attached and listening.

We go to code, set breakpoints by going to left of code number and clicking on it where a red dot appears. Code plays until it reaches breakpoint and stops so we can look inside of it.

We can hover over variables to see what is stored inside of them. We can also go to View and then Debug giving us special view of variables in all scopes like local, block, closure, global

We can also assign watchers that track state of variable and its value. We can also see the call stack
