# npm training note

## Help
- `npm -h` // command usage
- `npm <command> -h`
- `npm help <command>` // documentation
- `npm help-search <command>`
- `npm api-help` // When using as an API

## Install
- `npm i` === `npm install`
- `npm i -S` === `npm i --save`
- `npm i -D` === `npm in --save-dev`
See also [https://docs.npmjs.com/misc/config#shorthands-and-other-cli-niceties](https://docs.npmjs.com/misc/config#shorthands-and-other-cli-niceties)

## Scripts
- `npm start`
- `npm test`
- `npm run <taskname>`

## package.json
- `npm init`
- `npm init -y`
- `npm set init-author-name "Bradley Flood"` // `-email`, `-url`, ++ see [docs](https://docs.npmjs.com/misc/config#init-author-name)
- `npm config set proxy="http://localhost:3127"`
- `npm set` === `npm config set` || `npm get`
- `npm config delete proxy`
- `cat ~/.npmrc` // config settings

## Listing
- `ls node_modules/`
- `npm list` // tree
- `npm ls` === `npm list` || `npm la`
- `npm ls --depth 0`
- `npm ls --global` === `npm ls -g`
- `npm ls --long true` // info
- `npm ls --json true` // json

## Uninstall/Remove
- `npm uninstall <package>`
- `npm r` === `npm uninstall` || `npm un` || `npm rm`
- ...` -g`

## Versions
- `npm i express@4.15.2`
- `npm i express@4` === `npm i express@4.x.x`
- `npm i express@">=4.0.0 <4.15"
- `npm i express --save --save-exact` // Lock down exact version in package.json

## package.json dependencies versioning
```
"dependencies": {
    "express":"^4.15.2" // === `4.x.x`
    "express":"~4.15.2" // === `4.15.x`
    "express":"*" //  === `x` === latest
}
```

## Updating dependencies
- `npm update` // all in package.json
- `npm update <package>` // ie express
- `npm update -g` // global
- `npm update -g live-server`

## Installing via URL
- `npm i https://github.com/expressjs/express`
- `npm i https://bradleyflood.com/mypackage`
- `npm i gist:d38056f6602dcb536f413bb950ff3505`

