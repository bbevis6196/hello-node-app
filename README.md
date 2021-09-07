[README.md](https://github.com/bbevis6196/hello-node-app/files/7121294/README.md)
# hello-node-app
//First you check to see if Visual studio is installed

//Next you need to check if node.js is installed
    node -v

//Next Check if npm is installed
    npm -v

//Then you can start creating your test file to start your Server 

// Next you create node test.js
    console.log('hello node');

//Start server using 
    node test.js

//Next go to localhost:3001 allowing 'hello node' to be displayed on the webpage
//Next you create code to allow .get commands

//This code below Adds a function to call index.html to our server on localhost:3001 

const express = require('express')
const app = express()

app.get('/', function (req, res) {
res.send('Hello World')
})

app.get('/',  
    function(req, res)
    {
        res.sendFile('index.html', { root: __dirname }); 
    });

app.listen(3000) // I used Port 3001 on my server because i couldnt figure out what else was listening on port 3000

// Create index.html with basic html markup. Adding Any information you want. 

//Re-run the server from terminal with 
    node test.js 

//Refresh localhost:3001 and your webpage from index.html will be displayed

//At this point you can use this kinda like Apache allowing you to host a server you can connect to on local host and whatever port you are listening on.

//Would like to say I am so sorry for falling behind but WILL catch up!! Thanks
