# npmdoc-babar

#### api documentation for  babar (v0.1.0)  [![npm package](https://img.shields.io/npm/v/npmdoc-babar.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-babar) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-babar.svg)](https://travis-ci.org/npmdoc/node-npmdoc-babar)

#### CLI bar charts

[![NPM](https://nodei.co/npm/babar.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/babar)

- [https://npmdoc.github.io/node-npmdoc-babar/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-babar/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-babar/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-babar/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-babar/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-babar/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "babar",
    "version": "0.1.0",
    "description": "CLI bar charts",
    "main": "lib/babar.js",
    "scripts": {
        "build:lib": "coffee -o lib -c src/babar.coffee",
        "clean": "rimraf lib coverage",
        "preversion": "npm run clean",
        "version": "npm run build:lib",
        "postversion": "git push && git push --tags && npm run clean",
        "prepublish": "npm run clean && npm run build:lib",
        "dev": "coffee --watch -o lib/ -c src/babar.coffee",
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/stephan83/babar.git"
    },
    "keywords": [
        "cli",
        "bar",
        "charts",
        "graph",
        "ascii"
    ],
    "author": "Stephan Florquin",
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/stephan83/babar/issues"
    },
    "dependencies": {
        "colors": "~0.6.2"
    },
    "devDependencies": {
        "coffee-script": "~1.6.3",
        "rimraf": "^2.5.4"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
