---
templateKey: "blog-post"
title: "Javascript fetch"
date: 2021-08-27
featuredpost: true
featuredimage: /img/fetch.png
description: >-
  A simple fetch in Javascript and NodeJs
tags:
  - javascript
  - node
  - fetch
---

##Ways to fetch data
To get data from a local or external source in Javascript, we can use the [**Fetch Api**](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API) or in a NodeJs project, [**node-fetch**](https://www.npmjs.com/package/node-fetch#options) or [**axios**](https://www.npmjs.com/package/axios).
<br><br>

###Fetch Api

If we are working on the clientside, we can easily fetch our desired data by making use ofthe Fetch Api. <br>
The Fetch Api has a method, called **fetch()**, which allows us to do the fetching.

<br>

fetch() takes a **path** as its argument. <br>
Our path can be an external Url or a local directory.<br>
After the method is called, fetch() will make a **request** to the path and **return a promise**. <br>Then our promise will be resolved, for the case it was successful or for the case an error has occurred.
<br><br>

Here is an example for a simple fetch request.
<br><br>

For fetching a local image, the code could look like this:

```javascript{numberLines:true}

var myImage = document.querySelector(".my-image");

fetch("flowers.jpg")
.then(function (response) {
    if (!response.ok) {
        throw new Error("HTTP error, status = " + response.status);
    }
    return response.blob();
})
.then(function (myBlob) {
    var objectURL = URL.createObjectURL(myBlob);
    myImage.src = objectURL;
})
.catch(function (error) {
    var p = document.createElement("p");
    p.appendChild(document.createTextNode("Error: " + error.message));
    document.body.insertBefore(p, myImage);
});

```

<br>

To fetch data from an external Api, we would change the path of the fetch() method to:

<br>

```javascript{numberLines:true}{1-4}

fetch("https://fakestoreapi.com/img/71YAIFU48IL._AC_UL640_QL65_ML3_.jpg")
.then((res) => {
     return res.blob();
 })
.then(function (myBlob) {
    var objectURL = URL.createObjectURL(myBlob);
    myImage.src = objectURL;
})
.catch(function (error) {
    var p = document.createElement("p");
    p.appendChild(document.createTextNode("Error: " + error.message));
    document.body.insertBefore(p, myImage);
});

```

<br><br>

##Node-fetch

If we are instead working in a NodeJs project, we have to use another way to make a request and fetch the data. <br><br>
There are a couple of modules, that we can use, but today we will use the [node-fetch](https://www.npmjs.com/package/node-fetch#options) module, which is very similar to the Fetch Api. <br>
<br>
First we will need to install node-fetch like <br>
<br>

```markdown
npm install node-fetch
```

<br>

then we will need to import it

```javascript{numberLines:true}
const fetch = require("node-fetch");
```

<br>
if we want to work with JSON format, our code should look like

<br>

```javascript{numberLines:true}
fetch('https://api.github.com/users/github')
    .then(res => res.json())
    .then(json => console.log(json));
```

or for plain text or html

```javascript{numberLines:true}
fetch('https://github.com/')
    .then(res => res.text())
    .then(body => console.log(body));
```
