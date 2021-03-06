# npmdoc-cordova-plugin-qrscanner

#### api documentation for  [cordova-plugin-qrscanner (v2.5.0)](https://github.com/bitpay/cordova-plugin-qrscanner)  [![npm package](https://img.shields.io/npm/v/npmdoc-cordova-plugin-qrscanner.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cordova-plugin-qrscanner) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cordova-plugin-qrscanner.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cordova-plugin-qrscanner)

#### Fast, energy-efficient, highly-configurable QR code scanner.

[![NPM](https://nodei.co/npm/cordova-plugin-qrscanner.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/cordova-plugin-qrscanner)

- [https://npmdoc.github.io/node-npmdoc-cordova-plugin-qrscanner/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-cordova-plugin-qrscanner/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cordova-plugin-qrscanner/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cordova-plugin-qrscanner/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-cordova-plugin-qrscanner/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-cordova-plugin-qrscanner/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "cordova-plugin-qrscanner",
    "version": "2.5.0",
    "description": "Fast, energy-efficient, highly-configurable QR code scanner.",
    "cordova": {
        "id": "cordova-plugin-qrscanner",
        "platforms": [
            "ios"
        ]
    },
    "scripts": {
        "build": "gulp && npm run clean-build",
        "clean-build": "trash dist/plugin.min.js && trash dist/www.min.js && trash src/browser/worker.min.js",
        "test": "npm run jshint",
        "jshint": "jshint src/browser/src && jshint src/common/src && jshint tests",
        "gen-tests": "npm run build && npm run clean-platform-tests && npm run mkdirp-platform-tests && npm run copy-platform-tests && npm run install-platform-tests",
        "clean-platform-tests": "trash ../cordova-plugin-test-projects/cordova-plugin-qrscanner-tests",
        "mkdirp-platform-tests": "mkdirp ../cordova-plugin-test-projects/cordova-plugin-qrscanner-tests",
        "copy-platform-tests": "ncp tests/project ../cordova-plugin-test-projects/cordova-plugin-qrscanner-tests",
        "install-platform-tests": "cd ../cordova-plugin-test-projects/cordova-plugin-qrscanner-tests && npm install",
        "test:ios": "cd ../cordova-plugin-test-projects/cordova-plugin-qrscanner-tests && npm run test:ios",
        "test:android": "cd ../cordova-plugin-test-projects/cordova-plugin-qrscanner-tests && npm run test:android",
        "test:browser": "cd ../cordova-plugin-test-projects/cordova-plugin-qrscanner-tests && npm run test:browser",
        "test:windows": "cd ../cordova-plugin-test-projects/cordova-plugin-qrscanner-tests && npm run test:windows",
        "test:library": "npm run build && node tests/library/test.js",
        "changelog": "conventional-changelog -p angular -i CHANGELOG.md -s",
        "commitmsg": "validate-commit-msg",
        "prep-release": "git clean -dfx && npm install && npm run build && npm run changelog"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/bitpay/cordova-plugin-qrscanner"
    },
    "keywords": [
        "cordova",
        "qr",
        "qr code",
        "scanner",
        "reader",
        "ecosystem:cordova",
        "cordova-ios",
        "cordova-android",
        "cordova-browser",
        "UMD",
        "library",
        "electron",
        "NW.js"
    ],
    "author": "Jason Dreyzehner",
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/bitpay/cordova-plugin-qrscanner/issues"
    },
    "homepage": "https://github.com/bitpay/cordova-plugin-qrscanner",
    "dependencies": {
        "qrcode-reader": "^0.2.2",
        "webrtc-adapter": "^3.1.4"
    },
    "devDependencies": {
        "conventional-changelog-cli": "^1.2.0",
        "cz-conventional-changelog": "^1.1.6",
        "express": "^4.14.0",
        "gulp": "^3.9.1",
        "gulp-insert": "^0.5.0",
        "husky": "^0.13.1",
        "jshint": "^2.9.2",
        "mkdirp": "^0.5.1",
        "ncp": "^2.0.0",
        "raw-loader": "^0.5.1",
        "trash-cli": "^1.3.0",
        "validate-commit-msg": "^2.6.1",
        "webpack": "^2.1.0-beta.22"
    },
    "config": {
        "commitizen": {
            "path": "./node_modules/cz-conventional-changelog"
        },
        "validate-commit-msg": {
            "helpMessage": "\nThis project uses commitizen to document changes. Please try:\nnpm install commitizen -g && git cz\n"
        }
    },
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
