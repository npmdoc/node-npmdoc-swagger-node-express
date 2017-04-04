# api documentation for  [swagger-node-express (v2.1.3)](https://github.com/swagger-api/swagger-node-express)  [![npm package](https://img.shields.io/npm/v/npmdoc-swagger-node-express.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-swagger-node-express) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-swagger-node-express.svg)](https://travis-ci.org/npmdoc/node-npmdoc-swagger-node-express)
#### Wordnik swagger implementation for the express framework

[![NPM](https://nodei.co/npm/swagger-node-express.png?downloads=true)](https://www.npmjs.com/package/swagger-node-express)

[![apidoc](https://npmdoc.github.io/node-npmdoc-swagger-node-express/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-swagger-node-express_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-swagger-node-express/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-swagger-node-express/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-swagger-node-express/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tony Tam",
        "email": "fehguy@gmail.com",
        "url": "http://swagger.io"
    },
    "bugs": {
        "url": "https://github.com/swagger-api/swagger-node-express/issues"
    },
    "contributors": [
        {
            "name": "Pauh Hill",
            "email": "phill@kixeye.com"
        }
    ],
    "dependencies": {
        "lodash": "1.3.1"
    },
    "description": "Wordnik swagger implementation for the express framework",
    "devDependencies": {
        "cors": "2.1.1",
        "docco": "0.4.x",
        "express": "3.x",
        "jshint": "~2.3.0",
        "mocha": "~1.20.0",
        "once": "~1.3.0",
        "request": "~2.36.0",
        "should": "~4.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "4b1fee976e11284d276575911980b2258e379dab",
        "tarball": "https://registry.npmjs.org/swagger-node-express/-/swagger-node-express-2.1.3.tgz"
    },
    "engines": {
        "node": ">= 0.8.x"
    },
    "gitHead": "ade33c39a4a41e02bc18553a554717337ff45c13",
    "homepage": "https://github.com/swagger-api/swagger-node-express",
    "keywords": [
        "http",
        "rest",
        "swagger",
        "server"
    ],
    "license": "apache 2.0",
    "main": "index.js",
    "maintainers": [
        {
            "name": "wordnik",
            "email": "apiteam@wordnik.com"
        }
    ],
    "name": "swagger-node-express",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/swagger-api/swagger-node-express.git"
    },
    "scripts": {
        "pretest": "jshint lib",
        "start": "node sample-application/app.js",
        "test": "mocha -r should './test/**/*.js'"
    },
    "version": "2.1.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module swagger-node-express](#apidoc.module.swagger-node-express)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.</span>bodyParam (name, description, type, defaultValue, required)](#apidoc.element.swagger-node-express.bodyParam)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.</span>error (code, description)](#apidoc.element.swagger-node-express.error)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.</span>formParam (name, description, type, required, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.formParam)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.</span>headerParam (name, description, type, required)](#apidoc.element.swagger-node-express.headerParam)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.</span>pathParam (name, description, type, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.pathParam)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.</span>queryParam (name, description, type, required, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.queryParam)
1.  object <span class="apidocSignatureSpan">swagger-node-express.</span>allModels
1.  object <span class="apidocSignatureSpan">swagger-node-express.</span>apiInfo
1.  object <span class="apidocSignatureSpan">swagger-node-express.</span>appHandler
1.  object <span class="apidocSignatureSpan">swagger-node-express.</span>authorizations
1.  object <span class="apidocSignatureSpan">swagger-node-express.</span>errorHandling
1.  object <span class="apidocSignatureSpan">swagger-node-express.</span>getModels
1.  object <span class="apidocSignatureSpan">swagger-node-express.</span>paramTypes
1.  object <span class="apidocSignatureSpan">swagger-node-express.</span>params
1.  object <span class="apidocSignatureSpan">swagger-node-express.</span>resourceHelpers
1.  object <span class="apidocSignatureSpan">swagger-node-express.</span>resources
1.  object <span class="apidocSignatureSpan">swagger-node-express.</span>validators
1.  string <span class="apidocSignatureSpan">swagger-node-express.</span>apiVersion
1.  string <span class="apidocSignatureSpan">swagger-node-express.</span>basePath
1.  string <span class="apidocSignatureSpan">swagger-node-express.</span>formatString
1.  string <span class="apidocSignatureSpan">swagger-node-express.</span>jsonSuffix
1.  string <span class="apidocSignatureSpan">swagger-node-express.</span>resourcePath
1.  string <span class="apidocSignatureSpan">swagger-node-express.</span>swaggerVersion

#### [module swagger-node-express.errorHandling](#apidoc.module.swagger-node-express.errorHandling)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.errorHandling.</span>error (code, description)](#apidoc.element.swagger-node-express.errorHandling.error)

#### [module swagger-node-express.paramTypes](#apidoc.module.swagger-node-express.paramTypes)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.paramTypes.</span>body (name, description, type, defaultValue, required)](#apidoc.element.swagger-node-express.paramTypes.body)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.paramTypes.</span>form (name, description, type, required, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.paramTypes.form)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.paramTypes.</span>header (name, description, type, required)](#apidoc.element.swagger-node-express.paramTypes.header)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.paramTypes.</span>path (name, description, type, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.paramTypes.path)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.paramTypes.</span>q (name, description, type, required, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.paramTypes.q)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.paramTypes.</span>query (name, description, type, required, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.paramTypes.query)

#### [module swagger-node-express.resourceHelpers](#apidoc.module.swagger-node-express.resourceHelpers)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.resourceHelpers.</span>appendToApi (rootResource, api, spec)](#apidoc.element.swagger-node-express.resourceHelpers.appendToApi)
1.  [function <span class="apidocSignatureSpan">swagger-node-express.resourceHelpers.</span>wrap (callback, req, resp)](#apidoc.element.swagger-node-express.resourceHelpers.wrap)



# <a name="apidoc.module.swagger-node-express"></a>[module swagger-node-express](#apidoc.module.swagger-node-express)

#### <a name="apidoc.element.swagger-node-express.bodyParam"></a>[function <span class="apidocSignatureSpan">swagger-node-express.</span>bodyParam (name, description, type, defaultValue, required)](#apidoc.element.swagger-node-express.bodyParam)
- description and source-code
```javascript
bodyParam = function (name, description, type, defaultValue, required) {
  return {
    'name' : name,
    'description' : description,
    'type' : type,
    'required' : required || false,
    'paramType' : 'body',
    'defaultValue' : defaultValue
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swagger-node-express.error"></a>[function <span class="apidocSignatureSpan">swagger-node-express.</span>error (code, description)](#apidoc.element.swagger-node-express.error)
- description and source-code
```javascript
function error(code, description) {
  return {
    'code'   : code,
    'message': description
  };
}
```
- example usage
```shell
...
      'error': 'invalid param type ' + parameter.paramType
    });
    break;
  }
});

if (validationErrors.length > 0) {
  console.error(validationErrors);
  return;
}

if (!api.operations) {
  api.operations = [];
}
...
```

#### <a name="apidoc.element.swagger-node-express.formParam"></a>[function <span class="apidocSignatureSpan">swagger-node-express.</span>formParam (name, description, type, required, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.formParam)
- description and source-code
```javascript
formParam = function (name, description, type, required, allowableValuesEnum, defaultValue) {
  return {
    'name' : name,
    'description' : description,
    'type' : type,
    'required' : (typeof required !== 'undefined') ? required : true,
    'enum' : allowableValuesEnum,
    'paramType' : 'form',
    'defaultValue' : defaultValue
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swagger-node-express.headerParam"></a>[function <span class="apidocSignatureSpan">swagger-node-express.</span>headerParam (name, description, type, required)](#apidoc.element.swagger-node-express.headerParam)
- description and source-code
```javascript
headerParam = function (name, description, type, required) {
  return {
    'name' : name,
    'description' : description,
    'type' : type,
    'required' : required,
    'allowMultiple' : false,
    'paramType' : 'header'
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swagger-node-express.pathParam"></a>[function <span class="apidocSignatureSpan">swagger-node-express.</span>pathParam (name, description, type, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.pathParam)
- description and source-code
```javascript
pathParam = function (name, description, type, allowableValuesEnum, defaultValue) {
  return {
    'name' : name,
    'description' : description,
    'type' : type,
    'required' : true,
    'enum' : allowableValuesEnum,
    'paramType' : 'path',
    'defaultValue' : defaultValue
  };
}
```
- example usage
```shell
...
var findById = {
'spec': {
  "description" : "Operations about pets",
  "path" : "/pet.{format}/{petId}",
  "notes" : "Returns a pet based on ID",
  "summary" : "Find pet by ID",
  "method": "GET",
  "parameters" : [swagger.pathParam("petId", "ID of pet that needs to be fetched", "string")],
  "type" : "Pet",
  "errorResponses" : [swagger.errors.invalid('id'), swagger.errors.notFound('pet')],
  "nickname" : "getPetById"
},
'action': function (req,res) {
  if (!req.params.petId) {
    throw swagger.errors.invalid('id');
...
```

#### <a name="apidoc.element.swagger-node-express.queryParam"></a>[function <span class="apidocSignatureSpan">swagger-node-express.</span>queryParam (name, description, type, required, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.queryParam)
- description and source-code
```javascript
queryParam = function (name, description, type, required, allowableValuesEnum, defaultValue) {
  return {
    'name' : name,
    'description' : description,
    'type' : type,
    'required' : required,
    'enum' : allowableValuesEnum,
    'defaultValue' : defaultValue,
    'paramType' : 'query'
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swagger-node-express.errorHandling"></a>[module swagger-node-express.errorHandling](#apidoc.module.swagger-node-express.errorHandling)

#### <a name="apidoc.element.swagger-node-express.errorHandling.error"></a>[function <span class="apidocSignatureSpan">swagger-node-express.errorHandling.</span>error (code, description)](#apidoc.element.swagger-node-express.errorHandling.error)
- description and source-code
```javascript
function error(code, description) {
  return {
    'code'   : code,
    'message': description
  };
}
```
- example usage
```shell
...
      'error': 'invalid param type ' + parameter.paramType
    });
    break;
  }
});

if (validationErrors.length > 0) {
  console.error(validationErrors);
  return;
}

if (!api.operations) {
  api.operations = [];
}
...
```



# <a name="apidoc.module.swagger-node-express.paramTypes"></a>[module swagger-node-express.paramTypes](#apidoc.module.swagger-node-express.paramTypes)

#### <a name="apidoc.element.swagger-node-express.paramTypes.body"></a>[function <span class="apidocSignatureSpan">swagger-node-express.paramTypes.</span>body (name, description, type, defaultValue, required)](#apidoc.element.swagger-node-express.paramTypes.body)
- description and source-code
```javascript
body = function (name, description, type, defaultValue, required) {
  return {
    'name' : name,
    'description' : description,
    'type' : type,
    'required' : required || false,
    'paramType' : 'body',
    'defaultValue' : defaultValue
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swagger-node-express.paramTypes.form"></a>[function <span class="apidocSignatureSpan">swagger-node-express.paramTypes.</span>form (name, description, type, required, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.paramTypes.form)
- description and source-code
```javascript
form = function (name, description, type, required, allowableValuesEnum, defaultValue) {
  return {
    'name' : name,
    'description' : description,
    'type' : type,
    'required' : (typeof required !== 'undefined') ? required : true,
    'enum' : allowableValuesEnum,
    'paramType' : 'form',
    'defaultValue' : defaultValue
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swagger-node-express.paramTypes.header"></a>[function <span class="apidocSignatureSpan">swagger-node-express.paramTypes.</span>header (name, description, type, required)](#apidoc.element.swagger-node-express.paramTypes.header)
- description and source-code
```javascript
header = function (name, description, type, required) {
  return {
    'name' : name,
    'description' : description,
    'type' : type,
    'required' : required,
    'allowMultiple' : false,
    'paramType' : 'header'
  };
}
```
- example usage
```shell
...

### Allows special headers

If you want to modify the default headers sent with every swagger-managed method, you can do so as follows:

'''js
swagger.setHeaders = function setHeaders(res) {
  res.header("Access-Control-Allow-Headers", "Content-Type, X-API-KEY");
  res.header("Content-Type", "application/json; charset=utf-8");
};
'''
If you have a special name for an api key (such as 'X-API-KEY', per above), this is where you can inject it.

### Error handling
As of 2.1.0, swagger no longer consumes errors.  The preferred way to handle errors
...
```

#### <a name="apidoc.element.swagger-node-express.paramTypes.path"></a>[function <span class="apidocSignatureSpan">swagger-node-express.paramTypes.</span>path (name, description, type, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.paramTypes.path)
- description and source-code
```javascript
path = function (name, description, type, allowableValuesEnum, defaultValue) {
  return {
    'name' : name,
    'description' : description,
    'type' : type,
    'required' : true,
    'enum' : allowableValuesEnum,
    'paramType' : 'path',
    'defaultValue' : defaultValue
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swagger-node-express.paramTypes.q"></a>[function <span class="apidocSignatureSpan">swagger-node-express.paramTypes.</span>q (name, description, type, required, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.paramTypes.q)
- description and source-code
```javascript
q = function (name, description, type, required, allowableValuesEnum, defaultValue) {
  return {
    'name' : name,
    'description' : description,
    'type' : type,
    'required' : required,
    'enum' : allowableValuesEnum,
    'defaultValue' : defaultValue,
    'paramType' : 'query'
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swagger-node-express.paramTypes.query"></a>[function <span class="apidocSignatureSpan">swagger-node-express.paramTypes.</span>query (name, description, type, required, allowableValuesEnum, defaultValue)](#apidoc.element.swagger-node-express.paramTypes.query)
- description and source-code
```javascript
query = function (name, description, type, required, allowableValuesEnum, defaultValue) {
  return {
    'name' : name,
    'description' : description,
    'type' : type,
    'required' : required,
    'enum' : allowableValuesEnum,
    'defaultValue' : defaultValue,
    'paramType' : 'query'
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.swagger-node-express.resourceHelpers"></a>[module swagger-node-express.resourceHelpers](#apidoc.module.swagger-node-express.resourceHelpers)

#### <a name="apidoc.element.swagger-node-express.resourceHelpers.appendToApi"></a>[function <span class="apidocSignatureSpan">swagger-node-express.resourceHelpers.</span>appendToApi (rootResource, api, spec)](#apidoc.element.swagger-node-express.resourceHelpers.appendToApi)
- description and source-code
```javascript
function appendToApi(rootResource, api, spec) {
  var validationErrors = [];

  if (!spec.nickname || spec.nickname.indexOf(' ') >= 0) {
    //  nicknames don't allow spaces
    validationErrors.push({
      'path': api.path,
      'error': 'invalid nickname "' + spec.nickname + '"'
    });
  }
  // validate params
  _.forOwn(spec.parameters, function (parameter) {

    switch (parameter.paramType) {
    case 'path':
      if (api.path.indexOf('{' + parameter.name + '}') < 0) {
        validationErrors.push({
          'path': api.path,
          'name': parameter.name,
          'error': 'invalid path'
        });
      }
      break;
    case 'query':
      break;
    case 'body':
      break;
    case 'form':
      break;
    case 'header':
      break;
    default:
      validationErrors.push({
        'path': api.path,
        'name': parameter.name,
        'error': 'invalid param type ' + parameter.paramType
      });
      break;
    }
  });

  if (validationErrors.length > 0) {
    console.error(validationErrors);
    return;
  }

  if (!api.operations) {
    api.operations = [];
  }

  // TODO: replace if existing HTTP operation in same api path
  var op = {
    'parameters': spec.parameters,
    'method': spec.method,
    'notes': spec.notes,
    'responseMessages': spec.responseMessages,
    'nickname': spec.nickname,
    'summary': spec.summary,
    'consumes' : spec.consumes,
    'produces' : spec.produces
  };

  // Add custom fields.
  op = _.extend({}, spec, op);

  if (!spec.type) {
    op.type = 'void';
  }
  api.operations.push(op);

  if (!rootResource.models) {
    rootResource.models = {};
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.swagger-node-express.resourceHelpers.wrap"></a>[function <span class="apidocSignatureSpan">swagger-node-express.resourceHelpers.</span>wrap (callback, req, resp)](#apidoc.element.swagger-node-express.resourceHelpers.wrap)
- description and source-code
```javascript
function wrap(callback, req, resp) {
  callback(req, resp);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
