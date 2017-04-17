# api documentation for  [event-stream (v3.3.4)](http://github.com/dominictarr/event-stream)  [![npm package](https://img.shields.io/npm/v/npmdoc-event-stream.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-event-stream) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-event-stream.svg)](https://travis-ci.org/npmdoc/node-npmdoc-event-stream)
#### construct pipes of streams of events

[![NPM](https://nodei.co/npm/event-stream.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/event-stream)

- [https://npmdoc.github.io/node-npmdoc-event-stream/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-event-stream/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-event-stream/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-event-stream/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-event-stream/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-event-stream/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Dominic Tarr",
        "url": "http://bit.ly/dominictarr"
    },
    "bugs": {
        "url": "https://github.com/dominictarr/event-stream/issues"
    },
    "dependencies": {
        "duplexer": "~0.1.1",
        "from": "~0",
        "map-stream": "~0.1.0",
        "pause-stream": "0.0.11",
        "split": "0.3",
        "stream-combiner": "~0.0.4",
        "through": "~2.3.1"
    },
    "description": "construct pipes of streams of events",
    "devDependencies": {
        "asynct": "*",
        "it-is": "1",
        "stream-spec": "~0.3.5",
        "tape": "~2.3.0",
        "ubelt": "~3.2.2"
    },
    "directories": {},
    "dist": {
        "shasum": "4ab4c9a0f5a54db9338b4c34d86bfce8f4b35571",
        "tarball": "https://registry.npmjs.org/event-stream/-/event-stream-3.3.4.tgz"
    },
    "gitHead": "0d9d45744b06ead81976b3400569160b76299a41",
    "homepage": "http://github.com/dominictarr/event-stream",
    "license": "MIT",
    "maintainers": [
        {
            "name": "dominictarr"
        }
    ],
    "name": "event-stream",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/dominictarr/event-stream.git"
    },
    "scripts": {
        "prepublish": "npm ls && npm test",
        "test": "asynct test/",
        "test_tap": "set -e; for t in test/*.js; do node $t; done"
    },
    "testling": {
        "files": "test/*.js",
        "browsers": {
            "ie": [
                8,
                9
            ],
            "firefox": [
                13
            ],
            "chrome": [
                20
            ],
            "safari": [
                5.1
            ],
            "opera": [
                12
            ]
        }
    },
    "version": "3.3.4"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
