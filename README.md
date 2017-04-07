# api documentation for  [koa-route (v3.2.0)](https://github.com/koajs/route#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-koa-route.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-koa-route) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-koa-route.svg)](https://travis-ci.org/npmdoc/node-npmdoc-koa-route)
#### Koa route middleware

[![NPM](https://nodei.co/npm/koa-route.png?downloads=true)](https://www.npmjs.com/package/koa-route)

[![apidoc](https://npmdoc.github.io/node-npmdoc-koa-route/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-koa-route_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-koa-route/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-koa-route/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-koa-route/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/koajs/route/issues"
    },
    "dependencies": {
        "debug": "*",
        "methods": "~1.1.0",
        "path-to-regexp": "^1.2.0"
    },
    "description": "Koa route middleware",
    "devDependencies": {
        "istanbul-harmony": "0",
        "koa": "^2.0.0-alpha.3",
        "mocha": "^2.2.5",
        "should": "*",
        "supertest": "0"
    },
    "directories": {},
    "dist": {
        "shasum": "76298b99a6bcfa9e38cab6fe5c79a8733e758bce",
        "tarball": "https://registry.npmjs.org/koa-route/-/koa-route-3.2.0.tgz"
    },
    "files": [
        "index.js"
    ],
    "gitHead": "15408dcfea33b78dc1dd1e2b22af1cc860c6765a",
    "homepage": "https://github.com/koajs/route#readme",
    "keywords": [
        "koa",
        "middleware",
        "routes",
        "router",
        "route"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "aheckmann",
            "email": "aaron.heckmann+github@gmail.com"
        },
        {
            "name": "coderhaoxin",
            "email": "coderhaoxin@outlook.com"
        },
        {
            "name": "dead_horse",
            "email": "dead_horse@qq.com"
        },
        {
            "name": "eivifj",
            "email": "eivind.fjeldstad@gmail.com"
        },
        {
            "name": "fengmk2",
            "email": "fengmk2@gmail.com"
        },
        {
            "name": "jongleberry",
            "email": "jonathanrichardong@gmail.com"
        },
        {
            "name": "juliangruber",
            "email": "julian@juliangruber.com"
        },
        {
            "name": "tejasmanohar",
            "email": "me@tejas.io"
        },
        {
            "name": "tjholowaychuk",
            "email": "tj@vision-media.ca"
        },
        {
            "name": "travisjeffery",
            "email": "tj@travisjeffery.com"
        }
    ],
    "name": "koa-route",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/koajs/route.git"
    },
    "scripts": {
        "test": "NODE_ENV=test mocha --harmony --require should --reporter spec",
        "test-cov": "NODE_ENV=test node --harmony ./node_modules/.bin/istanbul cover ./node_modules/.bin/_mocha -- --require should",
        "test-travis": "NODE_ENV=test node --harmony ./node_modules/.bin/istanbul cover ./node_modules/.bin/_mocha --report lcovonly -- --require should"
    },
    "version": "3.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module koa-route](#apidoc.module.koa-route)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>acl (path, fn, opts)](#apidoc.element.koa-route.acl)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>all (path, fn, opts)](#apidoc.element.koa-route.all)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>bind (path, fn, opts)](#apidoc.element.koa-route.bind)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>checkout (path, fn, opts)](#apidoc.element.koa-route.checkout)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>connect (path, fn, opts)](#apidoc.element.koa-route.connect)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>copy (path, fn, opts)](#apidoc.element.koa-route.copy)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>del (path, fn, opts)](#apidoc.element.koa-route.del)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>delete (path, fn, opts)](#apidoc.element.koa-route.delete)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>get (path, fn, opts)](#apidoc.element.koa-route.get)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>head (path, fn, opts)](#apidoc.element.koa-route.head)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>link (path, fn, opts)](#apidoc.element.koa-route.link)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>lock (path, fn, opts)](#apidoc.element.koa-route.lock)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>m-search (path, fn, opts)](#apidoc.element.koa-route.m-search)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>merge (path, fn, opts)](#apidoc.element.koa-route.merge)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>mkactivity (path, fn, opts)](#apidoc.element.koa-route.mkactivity)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>mkcalendar (path, fn, opts)](#apidoc.element.koa-route.mkcalendar)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>mkcol (path, fn, opts)](#apidoc.element.koa-route.mkcol)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>move (path, fn, opts)](#apidoc.element.koa-route.move)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>notify (path, fn, opts)](#apidoc.element.koa-route.notify)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>options (path, fn, opts)](#apidoc.element.koa-route.options)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>patch (path, fn, opts)](#apidoc.element.koa-route.patch)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>post (path, fn, opts)](#apidoc.element.koa-route.post)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>propfind (path, fn, opts)](#apidoc.element.koa-route.propfind)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>proppatch (path, fn, opts)](#apidoc.element.koa-route.proppatch)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>purge (path, fn, opts)](#apidoc.element.koa-route.purge)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>put (path, fn, opts)](#apidoc.element.koa-route.put)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>rebind (path, fn, opts)](#apidoc.element.koa-route.rebind)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>report (path, fn, opts)](#apidoc.element.koa-route.report)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>search (path, fn, opts)](#apidoc.element.koa-route.search)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>subscribe (path, fn, opts)](#apidoc.element.koa-route.subscribe)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>trace (path, fn, opts)](#apidoc.element.koa-route.trace)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>unbind (path, fn, opts)](#apidoc.element.koa-route.unbind)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>unlink (path, fn, opts)](#apidoc.element.koa-route.unlink)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>unlock (path, fn, opts)](#apidoc.element.koa-route.unlock)
1.  [function <span class="apidocSignatureSpan">koa-route.</span>unsubscribe (path, fn, opts)](#apidoc.element.koa-route.unsubscribe)



# <a name="apidoc.module.koa-route"></a>[module koa-route](#apidoc.module.koa-route)

#### <a name="apidoc.element.koa-route.acl"></a>[function <span class="apidocSignatureSpan">koa-route.</span>acl (path, fn, opts)](#apidoc.element.koa-route.acl)
- description and source-code
```javascript
acl = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.all"></a>[function <span class="apidocSignatureSpan">koa-route.</span>all (path, fn, opts)](#apidoc.element.koa-route.all)
- description and source-code
```javascript
all = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.bind"></a>[function <span class="apidocSignatureSpan">koa-route.</span>bind (path, fn, opts)](#apidoc.element.koa-route.bind)
- description and source-code
```javascript
bind = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.checkout"></a>[function <span class="apidocSignatureSpan">koa-route.</span>checkout (path, fn, opts)](#apidoc.element.koa-route.checkout)
- description and source-code
```javascript
checkout = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.connect"></a>[function <span class="apidocSignatureSpan">koa-route.</span>connect (path, fn, opts)](#apidoc.element.koa-route.connect)
- description and source-code
```javascript
connect = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.copy"></a>[function <span class="apidocSignatureSpan">koa-route.</span>copy (path, fn, opts)](#apidoc.element.koa-route.copy)
- description and source-code
```javascript
copy = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.del"></a>[function <span class="apidocSignatureSpan">koa-route.</span>del (path, fn, opts)](#apidoc.element.koa-route.del)
- description and source-code
```javascript
del = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.delete"></a>[function <span class="apidocSignatureSpan">koa-route.</span>delete (path, fn, opts)](#apidoc.element.koa-route.delete)
- description and source-code
```javascript
delete = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.get"></a>[function <span class="apidocSignatureSpan">koa-route.</span>get (path, fn, opts)](#apidoc.element.koa-route.get)
- description and source-code
```javascript
get = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
...

# koa-route

 Uber simple route middleware for koa.

'''js
var _ = require('koa-route');
app.use(_.get('/pets', pets.list));
app.use(_.get('/pets/:name', pets.show));
'''

 If you need a full-featured solution check out [koa-router](https://github.com/alexmingoia/koa-router),
 a Koa clone of express-resource.

## Installation
...
```

#### <a name="apidoc.element.koa-route.head"></a>[function <span class="apidocSignatureSpan">koa-route.</span>head (path, fn, opts)](#apidoc.element.koa-route.head)
- description and source-code
```javascript
head = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.link"></a>[function <span class="apidocSignatureSpan">koa-route.</span>link (path, fn, opts)](#apidoc.element.koa-route.link)
- description and source-code
```javascript
link = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.lock"></a>[function <span class="apidocSignatureSpan">koa-route.</span>lock (path, fn, opts)](#apidoc.element.koa-route.lock)
- description and source-code
```javascript
lock = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.m-search"></a>[function <span class="apidocSignatureSpan">koa-route.</span>m-search (path, fn, opts)](#apidoc.element.koa-route.m-search)
- description and source-code
```javascript
m-search = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.merge"></a>[function <span class="apidocSignatureSpan">koa-route.</span>merge (path, fn, opts)](#apidoc.element.koa-route.merge)
- description and source-code
```javascript
merge = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.mkactivity"></a>[function <span class="apidocSignatureSpan">koa-route.</span>mkactivity (path, fn, opts)](#apidoc.element.koa-route.mkactivity)
- description and source-code
```javascript
mkactivity = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.mkcalendar"></a>[function <span class="apidocSignatureSpan">koa-route.</span>mkcalendar (path, fn, opts)](#apidoc.element.koa-route.mkcalendar)
- description and source-code
```javascript
mkcalendar = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.mkcol"></a>[function <span class="apidocSignatureSpan">koa-route.</span>mkcol (path, fn, opts)](#apidoc.element.koa-route.mkcol)
- description and source-code
```javascript
mkcol = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.move"></a>[function <span class="apidocSignatureSpan">koa-route.</span>move (path, fn, opts)](#apidoc.element.koa-route.move)
- description and source-code
```javascript
move = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.notify"></a>[function <span class="apidocSignatureSpan">koa-route.</span>notify (path, fn, opts)](#apidoc.element.koa-route.notify)
- description and source-code
```javascript
notify = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.options"></a>[function <span class="apidocSignatureSpan">koa-route.</span>options (path, fn, opts)](#apidoc.element.koa-route.options)
- description and source-code
```javascript
options = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.patch"></a>[function <span class="apidocSignatureSpan">koa-route.</span>patch (path, fn, opts)](#apidoc.element.koa-route.patch)
- description and source-code
```javascript
patch = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.post"></a>[function <span class="apidocSignatureSpan">koa-route.</span>post (path, fn, opts)](#apidoc.element.koa-route.post)
- description and source-code
```javascript
post = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.propfind"></a>[function <span class="apidocSignatureSpan">koa-route.</span>propfind (path, fn, opts)](#apidoc.element.koa-route.propfind)
- description and source-code
```javascript
propfind = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.proppatch"></a>[function <span class="apidocSignatureSpan">koa-route.</span>proppatch (path, fn, opts)](#apidoc.element.koa-route.proppatch)
- description and source-code
```javascript
proppatch = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.purge"></a>[function <span class="apidocSignatureSpan">koa-route.</span>purge (path, fn, opts)](#apidoc.element.koa-route.purge)
- description and source-code
```javascript
purge = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.put"></a>[function <span class="apidocSignatureSpan">koa-route.</span>put (path, fn, opts)](#apidoc.element.koa-route.put)
- description and source-code
```javascript
put = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.rebind"></a>[function <span class="apidocSignatureSpan">koa-route.</span>rebind (path, fn, opts)](#apidoc.element.koa-route.rebind)
- description and source-code
```javascript
rebind = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.report"></a>[function <span class="apidocSignatureSpan">koa-route.</span>report (path, fn, opts)](#apidoc.element.koa-route.report)
- description and source-code
```javascript
report = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.search"></a>[function <span class="apidocSignatureSpan">koa-route.</span>search (path, fn, opts)](#apidoc.element.koa-route.search)
- description and source-code
```javascript
search = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.subscribe"></a>[function <span class="apidocSignatureSpan">koa-route.</span>subscribe (path, fn, opts)](#apidoc.element.koa-route.subscribe)
- description and source-code
```javascript
subscribe = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.trace"></a>[function <span class="apidocSignatureSpan">koa-route.</span>trace (path, fn, opts)](#apidoc.element.koa-route.trace)
- description and source-code
```javascript
trace = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.unbind"></a>[function <span class="apidocSignatureSpan">koa-route.</span>unbind (path, fn, opts)](#apidoc.element.koa-route.unbind)
- description and source-code
```javascript
unbind = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.unlink"></a>[function <span class="apidocSignatureSpan">koa-route.</span>unlink (path, fn, opts)](#apidoc.element.koa-route.unlink)
- description and source-code
```javascript
unlink = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.unlock"></a>[function <span class="apidocSignatureSpan">koa-route.</span>unlock (path, fn, opts)](#apidoc.element.koa-route.unlock)
- description and source-code
```javascript
unlock = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.koa-route.unsubscribe"></a>[function <span class="apidocSignatureSpan">koa-route.</span>unsubscribe (path, fn, opts)](#apidoc.element.koa-route.unsubscribe)
- description and source-code
```javascript
unsubscribe = function (path, fn, opts){
  const re = pathToRegexp(path, opts);
  debug('%s %s -> %s', method || 'ALL', path, re);

  const createRoute = function(routeFunc){
    return function (ctx, next){
      // method
      if (!matches(ctx, method)) return next();

      // path
      const m = re.exec(ctx.path);
      if (m) {
        const args = m.slice(1).map(decode);
        ctx.routePath = path;
        debug('%s %s matches %s %j', ctx.method, path, ctx.path, args);
        args.unshift(ctx);
        args.push(next);
        return Promise.resolve(routeFunc.apply(ctx, args));
      }

      // miss
      return next();
    }
  };

  if (fn) {
    return createRoute(fn);
  } else {
    return createRoute;
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
