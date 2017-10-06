# Configuration for an npm package.

## Setup

 - from a npm package which is a git repository run 
```bash
  git submodule add https://github.com/harrysarson/js-config config
  npm install --save-dev chai eslint eslint-config-airbnb-base eslint-plugin-import mocha babel babel-preset-env
```
 - and then add the following to you package.json
```json
{
  "eslintConfig": {
    "extends": "./config/eslint.conf.js"
  },
  "babel": {
    "extends": "./config/babel.conf.json"
  }
}
```
