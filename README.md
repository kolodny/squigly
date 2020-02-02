# squigly
use ~ in require and import calls

## Important!
You must install `squigly` with a `~` alias which the usage below illustrates, otherwise the script won't run properly!

### install

```bash
npm install '~@https://github.com/kolodny/squigly#42783ea5' --save-dev
```

This module lets you turn things like `require('../../../../foo')` into something like  
`require('~/foo')`. The way it works is that on postinstall it replaces the `~` folder to point to the root of the project such that `app/node_modules/~` will point to `app/`
