var express = require('express');
var app = express();

app.use("/", express.static("webapp/"));

console.log("Server started on http://localhost:8000");

var portno = process.env.PORT || 8000;

app.listen(portno);