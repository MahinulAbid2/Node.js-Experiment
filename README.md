<b> PunchLine To Remember:</b> <br> The more information is added to the note, the more it is harder for me to understand the topic.
.... I think this is my issue.... as a programmer, I think I should build a habit of reading each and every word since finding bugs in code uses the same skills.

Focus on noting section wise. Which section comes after which section.
<br>
<br>


# Topic
* [What Can I Do with Node.js](#what-can-i-do-with-nodejs) <br>
* [Node.js Environment](#nodejs-environment) <br>
        i. [Execute JavaScript with Node.js](#execute-javascript-with-nodejs) <br>
        ii. [how can ](#creating-webpage-with-nodejs)



<br>



# What can I do with Node.js?

* Node.js can generate dynamic page content.
> Node.js can generate dynamic page content means that Node.js can `create web pages` with content that changes in real-time based on data, user input, or other factors. This allows for the creation of interactive and personalized web applications where the content isn't static but can be updated or customized on the fly.
* Node.js can create, open, read, write, delete, and close files on the server
* Node.js can collect form data
* Node.js can add, delete, modify data in your database

<br>

* Node.js can only execute JavaScript File.
* Node.js file can't execute HTML, CSS file but it can process and render file.

<br>

 ## Questions
* What task can I do with node.js?
* Can node.js work with MySQL?
* Is node.js syncronous or asyncronous?
* How PHP, ASP and node.js handles file?
* Can Node.js execute HTML file?

<br>

# RoadMap
![Screenshot 2023-09-15 212536](https://github.com/MahinulAbid2/Node.js-Experiment/assets/70069009/884c571e-46f9-4896-abc9-c590bfae903c)


<br>

# Node.js Environment Setup
* What is it: Node.js is an Environment which either lives `locally` in a computer, or in a `web server`.
* In order to work with node.js I have to install it on local computer.
* Go to https://nodejs.org/en/download
* Download, install Node.js exe file.
> No more extra work
* 

<br>

## Execute JavaScript with Node.js
* Create index.js file.
* Write some code in index.js file.
* Write this command in terminal:
```console
node index.js
```

![Screenshot 2023-09-15 195142](https://github.com/MahinulAbid2/Node.js-Experiment/assets/70069009/5b706a96-3e73-4b77-bff6-125a91bf8492)

Terminal is now acting as console. 

> Node.js is executing file only once.


<br>

<br>

# Fundamentals Of Node.js
* Adding Module to Project.

https://github.com/MahinulAbid2/Node.js-Experiment/assets/70069009/0d1e6a7d-077f-4b6d-89a2-248268e9c599


<br>
<br>

### Things needed to create Dynamic Webpage with Node.js
* `http` module
* `createServer()` function.

<br>



#### Http module 
* `Http module` gets included at the top of Node.js javascript file.

  <br>
  


```javascript
const http= require("http");
```
https://github.com/MahinulAbid2/Node.js-Experiment/assets/70069009/04d44e03-6388-41dc-b5fe-157edee27a43


* After including HTTP module in the project, I've unlocked some features of NODE.js.
* I can now `create server` using `HTTP` module.

<br>

### How to create server using HTTP module?

```javascript
var http = require('http');

//create a server object:
http.createServer(function (req, res) {
//here will be some operation related to the request and response according to the request.
}).listen(8080); //the server object listens on port 8080
```
<br>
<br>
<br>

### Alright. I have been talking about Node.js module. But what this node.js module actually is?

<details>
<summary> <ins> <b>Node.js Module (click to expand)</b> </ins></summary>


  # what is Node.js Module?

  * Up above in the example, first I used `const http = require('http');`
  * Fun Fact: The `require function` is specific to Node.js. I can not use it in normal javascript which runs in the browser.
  * Think this `http` as an object. If this `http` object has a method(function) name `greet`, How would I execute/call the method(function)?
  * `http.greet()` - this is how to call the method which is in http object.
  * <ins> Again, this is just imaginary example. </ins>

```javascript
const http= require("http");
// imported the http object.
// now that object has a method named "createServer()" which takes a function as parameter.

http.createServer("this takes an anonymous function as parameter");

http.createServer(("this anonymoys function takes two parameter")=>{});
// first parameter is the "request" parameter. which is an object.
// second parameter is "response" object.
// NOTE THAT: both the parameters are OBJECT.


``` 
</details>


<br>

### createServer
* What does createServer() method do?

