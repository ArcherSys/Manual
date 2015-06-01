# How to Host your Scratch Game

1. Copy the Embed code into an HTML file
2. Copy the HTML Code from the File
3. type this code
```
var http = require("http");
http.createServer(function(res,req){
res.writeHead(200, {"Content-Type":"text\html"});
res.end("YOUR HTML SCRATCH GAME CODE HERE");
}).listen(4001);
```

That is all there is to it!


