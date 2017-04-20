# npmdoc-swagger-node-express

#### api documentation for  swagger-node-express (v2.1.3)  [![npm package](https://img.shields.io/npm/v/npmdoc-swagger-node-express.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-swagger-node-express) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-swagger-node-express.svg)](https://travis-ci.org/npmdoc/node-npmdoc-swagger-node-express)

#### Wordnik swagger implementation for the express framework

[![NPM](https://nodei.co/npm/swagger-node-express.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/swagger-node-express)

- [https://npmdoc.github.io/node-npmdoc-swagger-node-express/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-swagger-node-express/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-swagger-node-express/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-swagger-node-express/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-swagger-node-express/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-swagger-node-express/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "swagger-node-express",
    "version": "2.1.3",
    "author": {
        "name": "Tony Tam",
        "url": "http://swagger.io"
    },
    "contributors": [
        {
            "name": "Pauh Hill"
        }
    ],
    "description": "Wordnik swagger implementation for the express framework",
    "repository": {
        "type": "git",
        "url": "https://github.com/swagger-api/swagger-node-express"
    },
    "keywords": [
        "http",
        "rest",
        "swagger",
        "server"
    ],
    "main": "index.js",
    "engines": {
        "node": ">= 0.8.x"
    },
    "dependencies": {
        "lodash": "1.3.1"
    },
    "devDependencies": {
        "express": "3.x",
        "docco": "0.4.x",
        "cors": "2.1.1",
        "mocha": "~1.20.0",
        "should": "~4.0.0",
        "once": "~1.3.0",
        "request": "~2.36.0",
        "jshint": "~2.3.0"
    },
    "license": "apache 2.0",
    "scripts": {
        "pretest": "jshint lib",
        "test": "mocha -r should './test/**/*.js'",
        "start": "node sample-application/app.js"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
