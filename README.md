# express_angular
express web application for angular and bower_bower_components ngRoute 

when i open up new cloud 9 how do I get start quicker. 

$npm init 
it will said 
name: (required)
version: 1.0.0 (enter)
keywords: (enter)
license: (enter)
is that ok? (enter)


open the file node_modules and delete socketio folder 

server.js
```
var http = require('http');
var path = require('path');
var async = require('async');
var express = require('express');
var router = express();
var server = http.createServer(router);

router.use(express.static(path.resolve(__dirname, 'client')));

server.listen(process.env.PORT || 3000, process.env.IP );
console.log("Localhost listening on port at " + 3000);
```

$ npm install express
$ npm install async
$ npm install -g bower (bower.io) 


deleted css folder not important. 
you will always want ui-router, not ng-route, why here is explaination... 
 
$ cd mkdir client
$ cd client

it will create new folder bower_components 
$bower install bootstrap 
$bower install font-awesome
$bower install angular-ui-bootstrap
$bower install angular-bootstrap 

either one 
$bower install angular-ui-router ['ui.router']
or 
$bower install angular-route  ['ngRoute']


when you are done with bower install 
go back cd ..
and npm start or npm server to start web server

create a new folder views, common, header.html, index1.html, and app.js 

using the bootsnipp.com and bootstrap example template 
http://getbootstrap.com/examples/carousel/
http://getbootstrap.com/examples/offcanvas/
