---
templateKey: "blog-post"
title: "Simple Node.js Project Set-up"
date: 2021-05-02
featuredpost: true
featuredimage: /img/Node.js_logo.png
description: >-
  In this tutorial we will set up Node.js with Express.js to display a simple "hello world" on the screen.
tags:
  - express
  - node
  - set-up
---

<!-- ##Set up a Node / Express Project -->

##Node.js

Node.js is a runtime environment, that lets us built web-applications, independent from the browser and the frontend.
<br><br>
It can handle server-side processes like collecting and modifying data as well as interacting with a database and much more.  
A fullstack – webapplication typically looks like this :  
<br>
`database – backend - frontend` <br>
<br>
one very popular tech-stack for example is :
<br><br>
`mongo.db – node.js – react`
<br><br>

###Set up the Node project

to start a node project we will first need to have [node](https://nodejs.org/en/download/) installed.
Then we will make use of the node package installer – **npm**, which comes with node. <br><br>
First let’s create a folder and open it in our text editor.
In the terminal, we can generate a new project by saying:

```javascript
npm init
```

or

```markdown
npm init -y
```

_(to skip confirming to the prompted questions)_<br><br>

this command will create a **package.json** file for us.<br>
So let's go ahead and do that.

###Package.json

The package.json file contains all the necessary information about our projects for example the packages, that we use and their version numbers, so even if the the version numbers change, we still know which ones we used and need for our project to work properly.
<br>
<br>
To built the project later **again**, we would only need to say:

`npm install`

and all the necessary packages would be installed from the package.json file.
<br><br>

At this point, we now have our package.json file in our folder.  
Let’s make another file and call it **app.js**.
<br><br>

###Modules in node.js
A great feature of Node.js is, that it is module-based. In other words you can use built-in modules, import third-party ones or even create your own, and split your functions into seperate files and routes.

To import a module, we use the **require()** method like:
<br><br>

`const module = require(„module“)`

<br>

the require() - method works like the **import function** in Vanilla Javascript. Actually you can use the Javascript import statement like in plain Javascript, since Node.js version 12, but you would need to configure it specifically in the package.json file and you wouldn’t be able import .json files for example. Thats why we will stick to the require() method instead.
<br><br>
There are a couple of useful built-in modules in Node.js like the **HTTP-module**, to transfer data or create a server, or the **URL- module**, to handle different paths of the web-adress. For more you can look them up [here](https://www.w3schools.com/nodejs/ref_modules.asp).
<br><br>
To add third-party packages, you can use this syntax in the terminal :
<br><br>
`npm install <package>`
<br><br>
Conveniently the package and all its dependecies will be added automatically to the package.json file. <br><br>
There are a lot of interesting node modules, that makes it so much easier to work with any part of building a web-application.  
To name a few, that you might find helpful, there is **nodemailer**, that lets you send emails from your computer or **dotenv** to handle environment variables, secret information that you might want to hide.
<br><br>
##Express.js
Now to set up our simple "hello world" application, we will use the Node.js framework **Express.js**.
<br><br>
Express is a lightweight and robust framework, that makes it easy to manage a server, handle routes, and HTTP requests.
<br><br>
To install express we type:
<br>

```markdown
npm install express
```

in our terminal.
<br><br>
Then we want to navigate to our app.js and **initialize** it. To do that we say:
<br><br>

```javascript{numberLines:true}
const express= require(„express“) //importing express
const app = express() //making an object of the express module
app.listen(3000, () => console.log(„app is listening on port 3000!“)) //creating a server on port 3000
```

our server is now located at `localhost:3000`.

<br>

###Routing in Express.js

To show our first message in the browser, we can make use of the routing feature of express.
<br>
The syntax looks like this:
<br><br>
`app.Method(Path, Handler)`
<br><br>

**Method** is an HTTP request method like GET, PUT, POST or DELETE,
**Path** is a route on the web-adress and **Handler** is a function.

Now we will update our code to look like this:

```javascript{numberLines: true}{4-6}

const express= require(„express“)

const app = express();
app.get("/", (req, res) => {
	res.send("Hello World!");
});
app.listen(3000, () => console.log("Example app listening on port 3000!"));
```

to explain the code: <br>
the get method here takes as its first argument a path, where to „get“ the information from, our path is **/** , which represents the root of our url so basically at **localhost:3000/**. The second argument is a **callback function**, that is called immediately after the first argument. Here the function has two parameters, which are typical in http data handling. The first parameter is the **request** (req), that we are making, the data that we are asking for and the **response** (res) is what we are respponding with/ sending.<br>
In our case we are looking at our path at „localhost:3000/“ and sending our response to display it on this adress.
<br><br>
to start the server we go back to our terminal and say:
<br><br>

```
node app.js

```

<br><br>
now we have our server running!
<br>The connection is alive under `http://localhost:3000` and ready to be viewed in the browser.
Now we should be able to see „hello world!“ on the page. <br>
**Congratulations!**
