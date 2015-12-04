# express_angular
express web application for angular, bower_bower_components and ngRoute 

How to get started. web server application

$npm init 
it will said 
name: (required)
version: 1.0.0 (enter)
keywords: (enter)
license: (enter)
is that ok? (enter)

server.js
<code>
var http = require('http');
var path = require('path');
var async = require('async');
var express = require('express');
var router = express();
var server = http.createServer(router);

router.use(express.static(path.resolve(__dirname, 'public')));

server.listen(process.env.PORT || 3000, process.env.IP );
console.log("Localhost listening on port at " + 3000);
</code

$ npm install express
$ npm install async
$ npm install -g bower (bower.io) 
 
$ cd mkdir public
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

using the bootsnipp.com and bootstrap example templates 
http://getbootstrap.com/examples/carousel/
http://getbootstrap.com/examples/offcanvas/
