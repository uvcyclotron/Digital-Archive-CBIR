This is the node.js app for client interface i.e. the interface where the querying happens.

- **node_modules** contains the node modules that need to be installed before running the code. All the required node modules are mentioned in `package.json` and can be installed using `npm install`.

- **public** contains the public javascripts and stylesheets. `public/script.js` contains the code for AJAX calls on clicking search buttons.

- **routes** contains node.js routes. `routes/index.js` contains the all-important code for search mechanism.

- **views** contains the `index.jade` file which can be manipulated to change the frontend of interface.

- **package.json** contains the required dependencies.

- **app.js** contains the driver code for running the app. Type `nodemon app` or `node app` to start the server at `localhost:8080`. Modify this file to change the server properties like listening port etc.
