### Reading 13

###### Local Storage

Whoa! This is a lot of information! Over the head! Let's get started.

Local storage is a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you.


Checking for HTML Storage:

if (Modernizr.localstorage) { // window.localStorage is available! } else { // no native support for HTML5 storage :( // maybe try dojox.storage or a third-party solution }

 

How to use HTML Storage:

var foo = localStorage["bar"];
// ...
localStorage["bar"] = foo;


There are a lot of other uses for HTML storage. We will start bringing API's and using SQL databases. Looks like 
we have a lot to learn going forward.
