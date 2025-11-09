# Worklog

## Part 1: "Hello World" with Node.js
The very first step was just to prove I could run JavaScript outside of the browser.

## The Code (app.js)
## JavaScript

console.log('Hello World!');

## How to Run It
- Open your terminal.

- Navigate to the folder containing app.js.

- Run the command:
Bash
node app.js
  
## What I Learned
- How to install Node.js on my computer.

- That I can run a .js file directly from my terminal.

- console.log() works in Node.js just like it does in the browser.

## Part 2: My First Web Server with Express
## The next step was to create a real server that listens for requests and sends back a response, just like a real website.

## The Code (server.js)
## JavaScript

const express = require('express');
const app = express();
const port = 3000;

// This creates a "route"
// When someone visits the homepage ('/'), send this response
app.get('/', (req, res) => {
  res.send('Hello World from my Express server!');
});

// This starts the server and makes it listen for requests on port 3000
app.listen(port, () => {
  console.log(`Server listening at http://localhost:${port}`);
});

## How to Run It
- Initialize the project: This creates a package.json file, which is needed to manage our project's "dependencies" (like Express).

Bash
npm init -y

## Install Express: This downloads the Express code into a new node_modules folder.

Bash

npm install express

## Start the server: This runs our server.js file.

Bash
node server.js

## What I Learned
- What a web server is (it's just a program that listens for requests).

- What dependencies are and how to use npm to install them.

- What require('express') does (it imports the code we installed).

- How to create a route with app.get().

What localhost and a port (like 3000) are.
