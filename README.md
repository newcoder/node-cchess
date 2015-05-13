# A Chinese Chess web application.  

## Here is how it works:

At the backend, node.js (or io.js) is used, node will load chess engine as child process. The node communicates with chess engine by UCI [Universal Chess Interface](http://en.wikipedia.org/wiki/Universal_Chess_Interface), the way that basically all chess UIs talk with chess engine. UCI is asychronous interface, so though the chess engine is CPU intensive, it can work with node perfectly. UCCI targets for Chinese chess, it is a variation of UCI with very little difference.  

The UI part, it's just a Single Page Application powered by Express, the web chess board is built with jQuery. 

UI talks with server via socket.io

## How to get it running:
- clone the rep
- make sure node module for Express are ready
````
npm install
````
- run server
````
node app
````
- open browser
````
http://localhost:3000/index.html
````

Enjoy!

MIT


