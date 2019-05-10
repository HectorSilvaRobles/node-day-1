## Node

- Student can create an index.js file
- Student can run a javascript file using node
- Student can run a javascript file using nodemon
- Student can describe that node is the V8 javascript engine
- Student can require and use other files in node

## Servers

- Student can describe the role of servers in a client-server model
- Student can identify the parts of code that listen to external requests

## NPM

- Student can npm init
- Student can npm install
- Student can npm install --save
- Student can describe the role of a package.json file
- Student can describe the purpose of the node_modules folder
- Student can .gitignore node_modules

## Express

- Student can install and require express
- Student can start a basic express server by creating an app and listening on a port
- Student can write the handler function with the correct parameters req, res and next
- Student can access url parameters on req.params
- Student can set up an endpoint path to expect multiple params
- Student can use req.query
- Student can send data back with res.send and res.json
- Student can set a status code with res.status


---

## Node

the v8 JavaScript engine that runs outside of the browser


**NPM:**

Node Package Manager

**package.json**

package.json is a config file for our application, it will have instructions on dependencies to download and how node should run your application.

https://docs.npmjs.com/files/package.json


**.gitignore**

tells git which files not to push to github
file/directories to be ignored

- node_modules
- .env (password file)
- anything you dont want on github

**server:**

computor or a device that provides a service to another computer

a webserver is a program that can handle incoming requests and repond accordingly,

manages access to a centerlized resource

todays centralized resoure: `data.json`

a computer program that accesses a service made available by a server

**client**

**params**
typically stand for a particular resource look like a normal path on the frontend

backend example:
params denoted with a "`:`"

```js
app.get('/api/:id')
```
access params in endpoint function handler

```js
req.params.id;
```

**query**

typically used to manipulate/search data being accessed

frontend example
denoted with a "`?`"

``` js
'http://localhost:4000/api/students?name=josh'
```

access query in endpoint function handler:

``` js
req.query.name;
```


## Server instructions

- mkdir server
- touch index.js .gitignore
- npm init -y
- add node_module => .gitignore
- npm i express
- require express
- declare app variable set = to express()
- declare port
- app.listen => port
- declare endpoint
- method - get
- path '/api/...
- handler => (req, res, next) => data to send
- test in browser
