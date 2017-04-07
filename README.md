# api documentation for  [postcss-import (v9.1.0)](https://github.com/postcss/postcss-import#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-postcss-import.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-postcss-import) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-postcss-import.svg)](https://travis-ci.org/npmdoc/node-npmdoc-postcss-import)
#### PostCSS plugin to import CSS files

[![NPM](https://nodei.co/npm/postcss-import.png?downloads=true)](https://www.npmjs.com/package/postcss-import)

[![apidoc](https://npmdoc.github.io/node-npmdoc-postcss-import/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-postcss-import_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-postcss-import/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-postcss-import/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-postcss-import/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Maxime Thirouin"
    },
    "bugs": {
        "url": "https://github.com/postcss/postcss-import/issues"
    },
    "dependencies": {
        "object-assign": "^4.0.1",
        "postcss": "^5.0.14",
        "postcss-value-parser": "^3.2.3",
        "promise-each": "^2.2.0",
        "read-cache": "^1.0.0",
        "resolve": "^1.1.7"
    },
    "description": "PostCSS plugin to import CSS files",
    "devDependencies": {
        "ava": "^0.16.0",
        "eslint": "^1.10.3",
        "eslint-config-i-am-meticulous": "^2.0.0",
        "npmpub": "^3.0.1",
        "postcss-scss": "^0.1.3",
        "sugarss": "^0.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "95fe9876a1e79af49fbdc3589f01fe5aa7cc1e80",
        "tarball": "https://registry.npmjs.org/postcss-import/-/postcss-import-9.1.0.tgz"
    },
    "eslintConfig": {
        "extends": "eslint-config-i-am-meticulous/es5"
    },
    "files": [
        "index.js",
        "lib"
    ],
    "gitHead": "2a687f867ba73e51aa9a838fa3f14e08174786f7",
    "homepage": "https://github.com/postcss/postcss-import#readme",
    "jspm": {
        "name": "postcss-import",
        "main": "index.js",
        "browser": {
            "./lib/load-content": "@empty",
            "./lib/resolve-id": "@empty"
        }
    },
    "keywords": [
        "css",
        "postcss",
        "postcss-plugin",
        "import",
        "node modules",
        "npm"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "moox",
            "email": "m@moox.io"
        },
        {
            "name": "ryanzim",
            "email": "opensrc@ryanzim.com"
        },
        {
            "name": "trysound",
            "email": "trysound@yandex.ru"
        }
    ],
    "name": "postcss-import",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/postcss/postcss-import.git"
    },
    "scripts": {
        "lint": "eslint --fix .",
        "pretest": "npm run lint",
        "release": "npmpub",
        "test": "ava"
    },
    "version": "9.1.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module postcss-import](#apidoc.module.postcss-import)
1.  [function <span class="apidocSignatureSpan">postcss-import.</span>process (root, opts)](#apidoc.element.postcss-import.process)



# <a name="apidoc.module.postcss-import"></a>[module postcss-import](#apidoc.module.postcss-import)

#### <a name="apidoc.element.postcss-import.process"></a>[function <span class="apidocSignatureSpan">postcss-import.</span>process (root, opts)](#apidoc.element.postcss-import.process)
- description and source-code
```javascript
process = function (root, opts) {
  return postcss([creator(opts)]).process(root, opts);
}
```
- example usage
```shell
...

// css to be processed
var css = fs.readFileSync("css/input.css", "utf8")

// process css
postcss()
  .use(atImport())
  .process(css, {
// 'from' option is required so relative import can work from input dirname
from: "css/input.css"
  })
  .then(function (result) {
var output = result.css

console.log(output)
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
