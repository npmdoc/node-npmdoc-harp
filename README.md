# api documentation for  [harp (v0.23.0)](http://harpjs.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-harp.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-harp) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-harp.svg)](https://travis-ci.org/npmdoc/node-npmdoc-harp)
#### Static web server with built in preprocessing

[![NPM](https://nodei.co/npm/harp.png?downloads=true)](https://www.npmjs.com/package/harp)

[![apidoc](https://npmdoc.github.io/node-npmdoc-harp/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-harp_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-harp/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-harp/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-harp/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Brock Whitten",
        "email": "brock@chloi.io"
    },
    "bin": {
        "harp": "./bin/harp"
    },
    "bugs": {
        "url": "http://github.com/sintaxi/harp/issues"
    },
    "contributors": [
        {
            "name": "Brock Whitten",
            "email": "brock@chloi.io"
        },
        {
            "name": "Rob Ellis",
            "email": "rob@chloi.io"
        },
        {
            "name": "Jorge Pedret",
            "email": "jorge@chloi.io"
        },
        {
            "name": "Michael Brooks",
            "email": "michael@michaelbrooks.ca"
        },
        {
            "name": "Tommy-Carlos Williams",
            "email": "tommy@devgeeks.org"
        },
        {
            "name": "Darryl Pogue",
            "email": "darryl@dpogue.ca"
        },
        {
            "name": "Boris Mann",
            "email": "boris@bmannconsulting.com"
        },
        {
            "name": "Kenneth Ormandy",
            "email": "kenneth@chloi.io"
        },
        {
            "name": "Keith Yao",
            "email": "i@yaofur.com"
        },
        {
            "name": "Eric Drechsel",
            "email": "eric@pdxhub.org"
        },
        {
            "name": "Andrew Hobden",
            "email": "andrew@hoverbear.org"
        },
        {
            "name": "Max Melentiev",
            "email": "printercu@gmail.com"
        },
        {
            "name": "Remy Sharp",
            "email": "remy@remysharp.com"
        },
        {
            "name": "Zeke Sikelianos",
            "email": "zeke@sikelianos.com"
        },
        {
            "name": "Marc Knaup",
            "email": "marc.knaup@koeln.de"
        },
        {
            "name": "Jurgen Van de Moere",
            "email": "jurgen.van.de.moere@gmail.com"
        }
    ],
    "dependencies": {
        "async": "0.2.9",
        "commander": "2.0.0",
        "connect": "2.30.2",
        "download-github-repo": "0.1.3",
        "envy-json": "0.2.1",
        "escape-html": "1.0.3",
        "fs-extra": "0.18.2",
        "mime": "1.2.11",
        "parseurl": "1.3.0",
        "pause": "0.1.0",
        "send": "0.13.0",
        "terraform": "1.3.0"
    },
    "description": "Static web server with built in preprocessing",
    "devDependencies": {
        "cheerio": "0.19.0",
        "mocha": "1.21.5",
        "nixt": "0.4.1",
        "request": "2.61.0",
        "should": "3.3.2"
    },
    "directories": {},
    "dist": {
        "shasum": "5db8493f8074cdf9bd478d336de7328729f3ff0b",
        "tarball": "https://registry.npmjs.org/harp/-/harp-0.23.0.tgz"
    },
    "engines": {
        "node": ">=0.12"
    },
    "gitHead": "7c0e02a7a150f713e0bdae316e889741aeaad83c",
    "homepage": "http://harpjs.com",
    "keywords": [
        "static web server",
        "static site generator",
        "sass",
        "less",
        "stylus",
        "markdown",
        "jade",
        "ejs",
        "coffeescript"
    ],
    "license": "MIT",
    "main": "./lib/index.js",
    "maintainers": [
        {
            "name": "kennethormandy",
            "email": "hello@kennethormandy.com"
        },
        {
            "name": "sintaxi",
            "email": "brock@sintaxi.com"
        }
    ],
    "name": "harp",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/sintaxi/harp.git"
    },
    "scripts": {
        "test": "mocha --reporter spec -t 8000"
    },
    "version": "0.23.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module harp](#apidoc.module.harp)
1.  [function <span class="apidocSignatureSpan">harp.</span>compile (projectPath, outputPath, callback)](#apidoc.element.harp.compile)
1.  [function <span class="apidocSignatureSpan">harp.</span>mount (mountPoint, root)](#apidoc.element.harp.mount)
1.  [function <span class="apidocSignatureSpan">harp.</span>multihost (dirPath, options, callback)](#apidoc.element.harp.multihost)
1.  [function <span class="apidocSignatureSpan">harp.</span>pipeline (root)](#apidoc.element.harp.pipeline)
1.  [function <span class="apidocSignatureSpan">harp.</span>server (dirPath, options, callback)](#apidoc.element.harp.server)
1.  object <span class="apidocSignatureSpan">harp.</span>helpers
1.  object <span class="apidocSignatureSpan">harp.</span>middleware
1.  object <span class="apidocSignatureSpan">harp.</span>pkg

#### [module harp.helpers](#apidoc.module.harp.helpers)
1.  [function <span class="apidocSignatureSpan">harp.helpers.</span>cssError (error)](#apidoc.element.harp.helpers.cssError)
1.  [function <span class="apidocSignatureSpan">harp.helpers.</span>ls (dir, callback)](#apidoc.element.harp.helpers.ls)
1.  [function <span class="apidocSignatureSpan">harp.helpers.</span>mimeType (source)](#apidoc.element.harp.helpers.mimeType)
1.  [function <span class="apidocSignatureSpan">harp.helpers.</span>normalizeUrl (url)](#apidoc.element.harp.helpers.normalizeUrl)
1.  [function <span class="apidocSignatureSpan">harp.helpers.</span>prime (primePath, options, callback)](#apidoc.element.harp.helpers.prime)
1.  [function <span class="apidocSignatureSpan">harp.helpers.</span>setup (projectPath, env)](#apidoc.element.harp.helpers.setup)
1.  [function <span class="apidocSignatureSpan">harp.helpers.</span>stacktrace (str, options)](#apidoc.element.harp.helpers.stacktrace)
1.  [function <span class="apidocSignatureSpan">harp.helpers.</span>willAllow (projectPath, outputPath)](#apidoc.element.harp.helpers.willAllow)
1.  [function <span class="apidocSignatureSpan">harp.helpers.</span>willCollide (projectPath, outputPath)](#apidoc.element.harp.helpers.willCollide)

#### [module harp.middleware](#apidoc.module.harp.middleware)
1.  [function <span class="apidocSignatureSpan">harp.middleware.</span>basicAuth (req, rsp, next)](#apidoc.element.harp.middleware.basicAuth)
1.  [function <span class="apidocSignatureSpan">harp.middleware.</span>fallback (req, rsp, next)](#apidoc.element.harp.middleware.fallback)
1.  [function <span class="apidocSignatureSpan">harp.middleware.</span>hostProjectFinder (dirPath)](#apidoc.element.harp.middleware.hostProjectFinder)
1.  [function <span class="apidocSignatureSpan">harp.middleware.</span>index (dirPath)](#apidoc.element.harp.middleware.index)
1.  [function <span class="apidocSignatureSpan">harp.middleware.</span>mwl (req, rsp, next)](#apidoc.element.harp.middleware.mwl)
1.  [function <span class="apidocSignatureSpan">harp.middleware.</span>notFound (req, rsp, next)](#apidoc.element.harp.middleware.notFound)
1.  [function <span class="apidocSignatureSpan">harp.middleware.</span>notMultihostURL (req, rsp, next)](#apidoc.element.harp.middleware.notMultihostURL)
1.  [function <span class="apidocSignatureSpan">harp.middleware.</span>poly (req, rsp, next)](#apidoc.element.harp.middleware.poly)
1.  [function <span class="apidocSignatureSpan">harp.middleware.</span>process (req, rsp, next)](#apidoc.element.harp.middleware.process)
1.  [function <span class="apidocSignatureSpan">harp.middleware.</span>regProjectFinder (projectPath)](#apidoc.element.harp.middleware.regProjectFinder)
1.  [function <span class="apidocSignatureSpan">harp.middleware.</span>setup (req, rsp, next)](#apidoc.element.harp.middleware.setup)
1.  [function <span class="apidocSignatureSpan">harp.middleware.</span>static (req, res, next)](#apidoc.element.harp.middleware.static)
1.  [function <span class="apidocSignatureSpan">harp.middleware.</span>underscore (req, rsp, next)](#apidoc.element.harp.middleware.underscore)



# <a name="apidoc.module.harp"></a>[module harp](#apidoc.module.harp)

#### <a name="apidoc.element.harp.compile"></a>[function <span class="apidocSignatureSpan">harp.</span>compile (projectPath, outputPath, callback)](#apidoc.element.harp.compile)
- description and source-code
```javascript
compile = function (projectPath, outputPath, callback){

<span class="apidocCodeCommentSpan">  /**
   * Both projectPath and outputPath are optional
   */
</span>
  if(!callback){
    callback   = outputPath
    outputPath = "www"
  }

  if(!outputPath){
    outputPath = "www"
  }


  /**
   * Setup all the paths and collect all the data
   */

  try{
    outputPath = path.resolve(projectPath, outputPath)
    var setup  = helpers.setup(projectPath, "production")
    var terra   = terraform.root(setup.publicPath, setup.config.globals)
  }catch(err){
    return callback(err)
  }


  /**
   * Protect the user (as much as possible) from compiling up the tree
   * resulting in the project deleting its own source code.
   */

  if(!helpers.willAllow(projectPath, outputPath)){
    return callback({
      type: "Invalid Output Path",
      message: "Output path cannot be greater then one level up from project path and must be in directory starting with '_' (underscore
).",
      projectPath: projectPath,
      outputPath: outputPath
    })
  }


  /**
   * Compile and save file
   */

  var compileFile = function(file, done){
    process.nextTick(function () {
      terra.render(file, function(error, body){
        if(error){
          done(error)
        }else{
          if(body){
            var dest = path.resolve(outputPath, terraform.helpers.outputPath(file))
            fs.mkdirp(path.dirname(dest), function(err){
              fs.writeFile(dest, body, done)
            })
          }else{
            done()
          }
        }
      })
    })
  }


  /**
   * Copy File
   *
   * TODO: reference ignore extensions from a terraform helper.
   */
  var copyFile = function(file, done){
    var ext = path.extname(file)
    if(!terraform.helpers.shouldIgnore(file) && [".jade", ".ejs", ".md", ".styl", ".less", ".scss", ".sass", ".coffee"].indexOf(
ext) === -1){
      var localPath = path.resolve(outputPath, file)
      fs.mkdirp(path.dirname(localPath), function(err){
        fs.copy(path.resolve(setup.publicPath, file), localPath, done)
      })
    }else{
      done()
    }
  }

  /**
   * Scan dir, Compile Less and Jade, Copy the others
   */

  helpers.prime(outputPath, { ignore: projectPath }, function(err){
    if(err) console.log(err)

    helpers.ls(setup.publicPath, function(err, results){
      async.each(results, compileFile, function(err){
        if(err){
          callback(err)
        }else{
          async.each(results, copyFile, function(err){
            setup.config['harp_version'] = pkg.version
            delete setup.config.globals
            callback(null, setup.config)
          })
        }
      })
    })
  })

}
```
- example usage
```shell
...
harp.server(projectPath [,args] [,callback])
'''

**Or** compile harp application

'''js
var harp = require("harp")
harp.compile(projectPath [,outputPath] [, callback])
'''

**Or** use as Connect/ExpressJS middleware

'''js
var express = require("express");
var harp = require("harp");
...
```

#### <a name="apidoc.element.harp.mount"></a>[function <span class="apidocSignatureSpan">harp.</span>mount (mountPoint, root)](#apidoc.element.harp.mount)
- description and source-code
```javascript
mount = function (mountPoint, root){

  if(!root){
    root = mountPoint
    mountPoint = null
  }else{
    var rx = new RegExp("^" + mountPoint)
  }

  var finder = middleware.regProjectFinder(root)

  return function(req, rsp, next){

    if(rx){
      if(!req.url.match(rx)) return next()
      var originalUrl = req.url
      req.url         = req.url.replace(rx, "/")
    }

    finder(req, rsp, function(){
      middleware.setup(req, rsp, function(){
        middleware.static(req, rsp, function(){
          middleware.poly(req, rsp, function(){
            middleware.process(req, rsp, function(){
              if(originalUrl) req.url = originalUrl
              next()
            })
          })
        })
      })
    })
  }
}
```
- example usage
```shell
...
var app = express();
'''

'''js
// Express 3
app.configure(function(){
  app.use(express.static(__dirname + "/public"));
  app.use(harp.mount(__dirname + "/public"));
});
'''

'''js
// Express 4

app.use(express.static(__dirname + "/public"));
...
```

#### <a name="apidoc.element.harp.multihost"></a>[function <span class="apidocSignatureSpan">harp.</span>multihost (dirPath, options, callback)](#apidoc.element.harp.multihost)
- description and source-code
```javascript
multihost = function (dirPath, options, callback){
  var app = connect()
  app.use(middleware.notMultihostURL)
  app.use(middleware.index(dirPath))
  app.use(middleware.hostProjectFinder(dirPath))
  app.use(middleware.setup)
  app.use(middleware.basicAuth)
  app.use(middleware.underscore)
  app.use(middleware.mwl)
  app.use(middleware.static)
  app.use(middleware.poly)
  app.use(middleware.process)
  app.use(middleware.fallback)
  app.listen(options.port || 9000, callback)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.pipeline"></a>[function <span class="apidocSignatureSpan">harp.</span>pipeline (root)](#apidoc.element.harp.pipeline)
- description and source-code
```javascript
pipeline = function (root){
  console.log("Deprecated, please use MOUNT instead, this will be removed in a future version.");
  var publicPath = path.resolve(root)
  var terra = terraform.root(publicPath)

  return function(req, rsp, next){
    var normalizedPath  = helpers.normalizeUrl(req.url)
    var priorityList    = terraform.helpers.buildPriorityList(normalizedPath)
    var sourceFile      = terraform.helpers.findFirstFile(publicPath, priorityList)

    if(!sourceFile) return next()

    terra.render(sourceFile, function(error, body){
      if(error) return next(error)
      if(!body) return next() // 404

      var outputType = terraform.helpers.outputType(sourceFile)
      var mimeType   = helpers.mimeType(outputType)
      var charset    = mime.charsets.lookup(mimeType)
      rsp.statusCode = 200
      rsp.setHeader('Content-Type', mimeType + (charset ? '; charset=' + charset : ''))
      rsp.setHeader('Content-Length', Buffer.byteLength(body, charset));
      rsp.end(body)
    })

  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.server"></a>[function <span class="apidocSignatureSpan">harp.</span>server (dirPath, options, callback)](#apidoc.element.harp.server)
- description and source-code
```javascript
server = function (dirPath, options, callback){
  var app = connect()
  app.use(middleware.regProjectFinder(dirPath))
  app.use(middleware.setup)
  app.use(middleware.basicAuth)
  app.use(middleware.underscore)
  app.use(middleware.mwl)
  app.use(middleware.static)
  app.use(middleware.poly)
  app.use(middleware.process)
  app.use(middleware.fallback)

  return app.listen(options.port || 9966, options.ip, function(){
    app.projectPath = dirPath
    callback.apply(app, arguments)
  })
}
```
- example usage
```shell
...

You may also use harp as a node library for compiling or running as a server.

Serve up a harp application...

'''js
var harp = require("harp")
harp.server(projectPath [,args] [,callback])
'''

**Or** compile harp application

'''js
var harp = require("harp")
harp.compile(projectPath [,outputPath] [, callback])
...
```



# <a name="apidoc.module.harp.helpers"></a>[module harp.helpers](#apidoc.module.harp.helpers)

#### <a name="apidoc.element.harp.helpers.cssError"></a>[function <span class="apidocSignatureSpan">harp.helpers.</span>cssError (error)](#apidoc.element.harp.helpers.cssError)
- description and source-code
```javascript
cssError = function (error){
  var body = '' +

  'body{' +
    'margin:0;' +
  '}' +

  'body:before {' +
    'display: block;'+
    'white-space: pre;' +
    'content: "'+ error.error.source +' -> ' + error.error.dest + ' (' + error.error.message + ') ' + error.error.filename + '";'+
    'color: #444;'+
    'background-color: #fefe96;' +
    'padding: 40px 40px;'+
    'margin: 0;'+
    'font-family: monospace;'+
    'font-size: 14px;'+
  '}'

  return body
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.helpers.ls"></a>[function <span class="apidocSignatureSpan">harp.helpers.</span>ls (dir, callback)](#apidoc.element.harp.helpers.ls)
- description and source-code
```javascript
ls = function (dir, callback) {
  walk(dir, function(err, results){
    var files = []
    results.map(function(file){ files.push(path.relative(dir, file)) })
    callback(null, files)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.helpers.mimeType"></a>[function <span class="apidocSignatureSpan">harp.helpers.</span>mimeType (source)](#apidoc.element.harp.helpers.mimeType)
- description and source-code
```javascript
mimeType = function (source){
  var ext = path.extname(source)

  if(['.jade', '.md', '.ejs'].indexOf(ext)  !== -1){
    return mime.lookup('html')
  }else if(['.less', '.styl', '.scss', '.sass'].indexOf(ext)  !== -1){
    return mime.lookup('css')
  } else if (['.js', '.coffee'].indexOf(ext) !== -1) {
    return mime.lookup('js')
  } else {
    return mime.lookup(source)
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.helpers.normalizeUrl"></a>[function <span class="apidocSignatureSpan">harp.helpers.</span>normalizeUrl (url)](#apidoc.element.harp.helpers.normalizeUrl)
- description and source-code
```javascript
normalizeUrl = function (url){

  // take off query string
  var base = unescape(url.split('?')[0])

<span class="apidocCodeCommentSpan">  /**
   * Normalize Path
   *
   * Note: This converts unix paths to windows path on windows
   * (not sure if this is a good thing)
   */
</span>  var file_path = path.normalize(base)

  // index.html support
  if (path.sep == file_path[file_path.length - 1]) file_path += 'index.html'

  return file_path
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.helpers.prime"></a>[function <span class="apidocSignatureSpan">harp.helpers.</span>prime (primePath, options, callback)](#apidoc.element.harp.helpers.prime)
- description and source-code
```javascript
prime = function (primePath, options, callback){

  if(!callback){
    callback = options
    options = {}
  }

<span class="apidocCodeCommentSpan">  /**
   * Options (only one)
   */
</span>  var ignorePath = options.ignore
    ? path.resolve(primePath, options.ignore)
    : null

  // Absolute paths are predictable.
  var primePath = path.resolve(primePath)

  fse.mkdirp(primePath, function(){
    fse.readdir(primePath, function(error, contents){

      /**
       * Delete each item in the directory in parallel. Thanks Ry!
       */

      if(contents.length == 0) return callback()

      var total = contents.length
      var count = 0


      contents.forEach(function(i){
        var filePath  = path.resolve(primePath, i)
        var gitRegExp = new RegExp(/^.git/)

        /**
         * We leave '.git', '.gitignore', and project path.
         */
        if(filePath === ignorePath || i.match(gitRegExp)){
          count++
          if(count == total) callback()
        }else{
          fse.remove(filePath, function(err){
            count++
            if(count == total) callback()
          })
        }
      })

    })
  })

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.helpers.setup"></a>[function <span class="apidocSignatureSpan">harp.helpers.</span>setup (projectPath, env)](#apidoc.element.harp.helpers.setup)
- description and source-code
```javascript
setup = function (projectPath, env){
  if(!env) env = "development"

  try{
    var configPath  = path.join(projectPath, "harp.json")
    var contents    = fs.readFileSync(configPath).toString()
    var publicPath  = path.join(projectPath, "public")
  }catch(e){
    try{
      var configPath  = path.join(projectPath, "_harp.json")
      var contents    = fs.readFileSync(configPath).toString()
      var publicPath  = projectPath
    }catch(e){
      var contents    = "{}"
      var publicPath  = projectPath
    }
  }

  // not sure what this does anymore.
  if(!contents || contents.replace(/^\s\s*/, '').replace(/\s\s*$/, '') == ''){
    contents = '{}'
  }

  // attempt to parse the file
  try{
    var cfg = JSON.parse(contents)
  }catch(e){
    e.source    = "JSON"
    e.dest      = "CONFIG"
    e.message   = e.message
    e.filename  = configPath
    e.stack     = contents
    e.lineno    = -1
    throw new terraform.helpers.TerraformError(e)
  }

  if(!cfg.hasOwnProperty('globals')) cfg['globals'] = {}

  cfg.globals.environment = process.env.NODE_ENV || env

  // replace values that look like environment variables
  // e.g. '$foo' -> process.env.foo
  cfg = envy(cfg)

  return {
    projectPath : projectPath,
    publicPath  : publicPath,
    config      : cfg
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.helpers.stacktrace"></a>[function <span class="apidocSignatureSpan">harp.helpers.</span>stacktrace (str, options)](#apidoc.element.harp.helpers.stacktrace)
- description and source-code
```javascript
stacktrace = function (str, options){
  var lineno  = options.lineno  || -1
  var context = options.context || 8
  var context = context = context / 2
  var lines   = ('\n' + str).split('\n')
  var start   = Math.max(lineno - context, 1)
  var end     = Math.min(lines.length, lineno + context)

  if(lineno === -1) end = lines.length

  var pad     = end.toString().length

  var context = lines.slice(start, end).map(function(line, i){
    var curr = i + start
    return (curr == lineno ? ' > ' : '   ')
      + Array(pad - curr.toString().length + 1).join(' ')
      + curr
      + '| '
      + line
  }).join('\n')

  return context
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.helpers.willAllow"></a>[function <span class="apidocSignatureSpan">harp.helpers.</span>willAllow (projectPath, outputPath)](#apidoc.element.harp.helpers.willAllow)
- description and source-code
```javascript
willAllow = function (projectPath, outputPath){
  var projectPath   = path.resolve(projectPath)
  var outputPath    = path.resolve(outputPath)
  var relativePath  = path.relative(projectPath, outputPath)
  var arr           = relativePath.split(path.sep)

  if(willCollide(projectPath, outputPath)){
    if(relativePath === ".."){
      if(projectPath.split(path.sep)[projectPath.split(path.sep).length - 1][0] == "_"){
        return true
      }else{
        return false
      }
    }else{
      return false
    }
  }else{
    return true
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.helpers.willCollide"></a>[function <span class="apidocSignatureSpan">harp.helpers.</span>willCollide (projectPath, outputPath)](#apidoc.element.harp.helpers.willCollide)
- description and source-code
```javascript
willCollide = function (projectPath, outputPath){
  var projectPath   = path.resolve(projectPath)
  var outputPath    = path.resolve(outputPath)
  var relativePath  = path.relative(projectPath, outputPath)
  var arr           = relativePath.split(path.sep)
  var result        = true;

  arr.forEach(function(i){
    if(i !== "..") result = false
  })

<span class="apidocCodeCommentSpan">  /**
   * for @kennethormandy ;)
   */
</span>  if ([path.sep, "C:\\"].indexOf(outputPath) !== -1) result = true

  /**
   * For #400
   */
  if (projectPath === outputPath) result = true

  return result
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.harp.middleware"></a>[module harp.middleware](#apidoc.module.harp.middleware)

#### <a name="apidoc.element.harp.middleware.basicAuth"></a>[function <span class="apidocSignatureSpan">harp.middleware.</span>basicAuth (req, rsp, next)](#apidoc.element.harp.middleware.basicAuth)
- description and source-code
```javascript
basicAuth = function (req, rsp, next){

  // default empty
  var creds = []

  // allow array
  if(req.setup.config.hasOwnProperty("basicAuth") && req.setup.config["basicAuth"] instanceof Array)
    creds = req.setup.config["basicAuth"]

  // allow string
  if(req.setup.config.hasOwnProperty("basicAuth") && typeof req.setup.config["basicAuth"] === 'string')
    creds = [req.setup.config["basicAuth"]]

  // move on if no creds
  if(creds.length === 0) return next()

  // use connect auth lib iterate over all creds provided
  connect.basicAuth(function(user, pass){
    return creds.some(function(cred){
      return cred === user + ":" + pass
    })
  })(req, rsp, next)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.middleware.fallback"></a>[function <span class="apidocSignatureSpan">harp.middleware.</span>fallback (req, rsp, next)](#apidoc.element.harp.middleware.fallback)
- description and source-code
```javascript
fallback = function (req, rsp, next){
  skin(req, rsp, [custom200static, custom200dynamic, notFound], next)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.middleware.hostProjectFinder"></a>[function <span class="apidocSignatureSpan">harp.middleware.</span>hostProjectFinder (dirPath)](#apidoc.element.harp.middleware.hostProjectFinder)
- description and source-code
```javascript
hostProjectFinder = function (dirPath){
  return function(req, rsp, next){
    var host        = req.headers.host;
    var hostname    = host.split(':')[0];
    var matches     = [];

    fs.readdir(dirPath, function(err, files){
      var appPart = hostname.split(".")[0];
      files.forEach(function(file){
        var fp = file.split('.');
        var filePart;
        // Check against Reserved Domains first.
        if (fp.length > 2) {
          var domain = fp.slice(Math.max(fp.length - 2, 1)).join(".");
          if (reservedDomains.indexOf(domain) != -1) {
            fp = fp.slice(0, Math.max(fp.length - 2))
          }
        }

        filePart = fp.join("_");
        if (appPart == filePart) {
          matches.push(file);
        }
      });

      if(matches.length > 0){
        req.projectPath = path.resolve(dirPath, matches[0]);
        next();
      } else {
        rsp.end("Cannot find project")
      }

    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.middleware.index"></a>[function <span class="apidocSignatureSpan">harp.middleware.</span>index (dirPath)](#apidoc.element.harp.middleware.index)
- description and source-code
```javascript
index = function (dirPath){
  return function(req, rsp, next){
    var host      = req.headers.host;
    var hostname  = host.split(':')[0];
    var arr       = hostname.split(".");
    var port      = host.split(':')[1] ? ':' + host.split(':')[1] : '';
    var poly      = terraform.root(__dirname + "/templates");

    if(arr.length == 2){
      fs.readdir(dirPath, function(err, files){
        var projects = [];

        files.forEach(function(file){
          var local = file.split('.');

          var appPart = local.join("_");

          if (local.length > 2) {
            var domain = local.slice(Math.max(local.length - 2, 1)).join(".");
            if (reservedDomains.indexOf(domain) != -1) {
              appPart =  local[0];
            }
          }

          // DOT files are ignored.
          if (file[0] !== ".") {
            projects.push({
              "name"      : file,
              "localUrl"  : 'http://' + appPart + "." + host,
              "localPath" : path.resolve(dirPath, file)
            });
          }
        });

        poly.render("index.jade", { pkg: pkg, projects: projects, layout: "_layout.jade" }, function(error, body){
          rsp.end(body)
        });
      })
    } else {
      next();
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.middleware.mwl"></a>[function <span class="apidocSignatureSpan">harp.middleware.</span>mwl (req, rsp, next)](#apidoc.element.harp.middleware.mwl)
- description and source-code
```javascript
mwl = function (req, rsp, next){
  var ext = path.extname(req.url).replace(/^\./, '')
  req.originalExt = ext

  // This prevents the source files from being served, but also
  // has to factor in that in this brave new world, sometimes
  // '.html' (Handlebars, others), '.css' (PostCSS), and
  // '.js' (Browserify) are actually being used to specify
  // source files

  //if (['js'].indexOf(ext) === -1) {
    if (terraform.helpers.processors["html"].indexOf(ext) !== -1 || terraform.helpers.processors["css"].indexOf(ext) !== -1 || terraform
.helpers.processors["js"].indexOf(ext) !== -1) {
      notFound(req, rsp, next)
    } else {
      next()
    }
  //} else {
    //next()
  //}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.middleware.notFound"></a>[function <span class="apidocSignatureSpan">harp.middleware.</span>notFound (req, rsp, next)](#apidoc.element.harp.middleware.notFound)
- description and source-code
```javascript
notFound = function (req, rsp, next){
  skin(req, rsp, [custom404static, custom404dynamic, default404], next)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.middleware.notMultihostURL"></a>[function <span class="apidocSignatureSpan">harp.middleware.</span>notMultihostURL (req, rsp, next)](#apidoc.element.harp.middleware.notMultihostURL)
- description and source-code
```javascript
notMultihostURL = function (req, rsp, next){
  var host      = req.headers.host
  var hostname  = host.split(':')[0]
  var arr       = hostname.split(".")
  var port      = host.split(':')[1] ? ':' + host.split(':')[1] : ''

  if(hostname == "127.0.0.1" || hostname == "localhost"){
    rsp.statusCode = 307
    rsp.setHeader('Location', 'http://harp.nu' + port)
    rsp.end("redirecting you to http://harp.nu" + port)
  }else if(arr.length == 4){
    arr.pop()
    arr.push('io')
    var link = 'http://' + arr.join('.') + port
    var body = "Local server does not support history. Perhaps you are looking for <href='" + link + "'>" + link + "</a>."
    rsp.statusCode = 307
    rsp.end(body)
  }else if(arr.length > 4){
    arr.shift()
    var link = 'http://' + arr.join('.') + port
    rsp.statusCode = 307
    rsp.setHeader('Location', link)
    rsp.end("redirecting you to " + link)
  }else{
    next()
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.middleware.poly"></a>[function <span class="apidocSignatureSpan">harp.middleware.</span>poly (req, rsp, next)](#apidoc.element.harp.middleware.poly)
- description and source-code
```javascript
poly = function (req, rsp, next){
  if(req.hasOwnProperty("poly")) return next()

  try{
    req.poly = terraform.root(req.setup.publicPath, req.setup.config.globals)
  }catch(error){
    error.stack = helpers.stacktrace(error.stack, { lineno: error.lineno })
    var locals = {
      project: req.headers.host,
      error: error,
      pkg: pkg
    }
    return terraform.root(__dirname + "/templates").render("error.jade", locals, function(err, body){
      rsp.statusCode = 500
      rsp.end(body)
    })
  }
  next()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.middleware.process"></a>[function <span class="apidocSignatureSpan">harp.middleware.</span>process (req, rsp, next)](#apidoc.element.harp.middleware.process)
- description and source-code
```javascript
process = function (req, rsp, next){
  var normalizedPath  = helpers.normalizeUrl(req.url)
  var priorityList    = terraform.helpers.buildPriorityList(normalizedPath)
  var sourceFile      = terraform.helpers.findFirstFile(req.setup.publicPath, priorityList)


<span class="apidocCodeCommentSpan">  /**
   * We GTFO if we don't have a source file.
   */
</span>
  if(!sourceFile){
    if (path.basename(normalizedPath) === "index.html") {
      var pathAr = normalizedPath.split(path.sep); pathAr.pop() // Pop index.html off the list
      var prospectCleanPath       = pathAr.join("/")
      var prospectNormalizedPath  = helpers.normalizeUrl(prospectCleanPath)
      var prospectPriorityList    = terraform.helpers.buildPriorityList(prospectNormalizedPath)
      prospectPriorityList.push(path.basename(prospectNormalizedPath + ".html"))

      sourceFile = terraform.helpers.findFirstFile(req.setup.publicPath, prospectPriorityList)

      if (!sourceFile) {
        return next()
      } else {
        // 301 redirect
        rsp.statusCode = 301
        rsp.setHeader('Location', prospectCleanPath)
        rsp.end('Redirecting to ' + utilsEscape(prospectCleanPath))
      }

    } else {
      return next()
    }
  } else {

    /**
     * Now we let terraform handle the asset pipeline.
     */

    req.poly.render(sourceFile, function(error, body){
      if(error){
        error.stack = helpers.stacktrace(error.stack, { lineno: error.lineno })

        var locals = {
          project: req.headers.host,
          error: error,
          pkg: pkg
        }
        if(terraform.helpers.outputType(sourceFile) == 'css'){
          var outputType = terraform.helpers.outputType(sourceFile)
          var mimeType   = helpers.mimeType(outputType)
          var charset    = mime.charsets.lookup(mimeType)
          var body       = helpers.cssError(locals)
          rsp.statusCode = 200
          rsp.setHeader('Content-Type', mimeType + (charset ? '; charset=' + charset : ''))
          rsp.setHeader('Content-Length', Buffer.byteLength(body, charset));
          rsp.end(body)
        }else{

          // Make the paths relative but keep the root dir.
          // TODO: move to helper.
          //
          // var loc = req.projectPath.split(path.sep); loc.pop()
          // var loc = loc.join(path.sep) + path.sep
          // if(error.filename) error.filename = error.filename.replace(loc, "")

          terraform.root(__dirname + "/templates").render("error.jade", locals, function(err, body){
            var mimeType   = helpers.mimeType('html')
            var charset    = mime.charsets.lookup(mimeType)
            rsp.statusCode = 500
            rsp.setHeader('Content-Type', mimeType + (charset ? '; charset=' + charset : ''))
            rsp.setHeader('Content-Length', Buffer.byteLength(body, charset));
            rsp.end(body)
          })
        }
      }else{
        // 404
        if(!body) return next()

        var outputType = terraform.helpers.outputType(sourceFile)
        var mimeType   = helpers.mimeType(outputType)
        var charset    = mime.charsets.lookup(mimeType)
        rsp.statusCode = 200
        rsp.setHeader('Content-Type', mimeType + (charset ? '; charset=' + charset : ''))
        rsp.setHeader('Content-Length', Buffer.byteLength(body, charset));
        rsp.end(body);
      }
    })
  }










}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.middleware.regProjectFinder"></a>[function <span class="apidocSignatureSpan">harp.middleware.</span>regProjectFinder (projectPath)](#apidoc.element.harp.middleware.regProjectFinder)
- description and source-code
```javascript
regProjectFinder = function (projectPath){
  return function(req, rsp, next){
    req.projectPath = projectPath
    next()
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.middleware.setup"></a>[function <span class="apidocSignatureSpan">harp.middleware.</span>setup (req, rsp, next)](#apidoc.element.harp.middleware.setup)
- description and source-code
```javascript
setup = function (req, rsp, next){
  if(req.hasOwnProperty('setup')) return next()

  try{
    req.setup = helpers.setup(req.projectPath)
  }catch(error){
    error.stack = helpers.stacktrace(error.stack, { lineno: error.lineno })

    var locals = {
      project: req.headers.host,
      error: error,
      pkg: pkg
    }

    return terraform.root(__dirname + "/templates").render("error.jade", locals, function(err, body){
      rsp.statusCode = 500
      rsp.end(body)
    })
  }

  next()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.harp.middleware.static"></a>[function <span class="apidocSignatureSpan">harp.middleware.</span>static (req, res, next)](#apidoc.element.harp.middleware.static)
- description and source-code
```javascript
static = function (req, res, next) {
  var options  = {}
  var redirect = true

  if ('GET' != req.method && 'HEAD' != req.method) return next()
  //if (['js'].indexOf(path.extname(req.url).replace(/^\./, '')) !== -1) return next()

  var pathn = parse(req).pathname;
  var pause = utilsPause(req);

  function resume() {
    next();
    pause.resume();
  }

  function directory() {

    if (!redirect) return resume();
    var pathname = url.parse(req.originalUrl).pathname;
    res.statusCode = 301;
    res.setHeader('Location', pathname + '/');
    res.end('Redirecting to ' + utilsEscape(pathname) + '/');
  }

  function error(err) {
    if (404 == err.status){
      // look for implicit '*.html' if we get a 404
      return path.extname(err.path) === ''
        ? serve(pathn + ".html")
        : resume()
    }
    next(err);
  }

  var serve = function(pathn){
    send(req, pathn, {
        maxage: options.maxAge || 0,
        root: req.setup.publicPath,
        hidden: options.hidden
      })
      .on('error', error)
      .on('directory', directory)
      .pipe(res)
  }
  serve(pathn)
}
```
- example usage
```shell
...
var harp = require("harp");
var app = express();
'''

'''js
// Express 3
app.configure(function(){
  app.use(express.static(__dirname + "/public"));
  app.use(harp.mount(__dirname + "/public"));
});
'''

'''js
// Express 4
...
```

#### <a name="apidoc.element.harp.middleware.underscore"></a>[function <span class="apidocSignatureSpan">harp.middleware.</span>underscore (req, rsp, next)](#apidoc.element.harp.middleware.underscore)
- description and source-code
```javascript
underscore = function (req, rsp, next){
  if(terraform.helpers.shouldIgnore(req.url)){
    notFound(req, rsp, next)
  }else{
    next()
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
