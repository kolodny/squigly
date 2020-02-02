# squigly
use ~ in require and import calls

[![NPM version][npm-image]][npm-url]
[![Downloads][downloads-image]][downloads-url]

## Important!
You must install `squigly` with a `~` alias which the usage below illustrates, otherwise the script won't run properly!

### install

```bash
npm install ~@squigly --save-dev
```

This module lets you turn things like `require('../../../../foo')` into something like  
`require('~/foo')`. The way it works is that on postinstall it replaces the `~` folder to point to the root of the project such that `app/node_modules/~` will point to `app/`

[npm-image]: https://img.shields.io/npm/v/squigly.svg?style=flat-square
[npm-url]: https://npmjs.org/package/squigly
[downloads-image]: http://img.shields.io/npm/dm/squigly.svg?style=flat-square
[downloads-url]: https://npmjs.org/package/squigly