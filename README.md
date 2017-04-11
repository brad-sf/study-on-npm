# NPM Training Notes

## Install
- `npm i` === `npm install`
- `npm i -S` === `npm i --save`
- `npm i -D` === `npm in --save-dev`
See also [https://docs.npmjs.com/misc/config#shorthands-and-other-cli-niceties](https://docs.npmjs.com/misc/config#shorthands-and-other-cli-niceties)

## Scripts
- `npm start`
- `npm test`
- `npm run <taskname>`

## Help
- `npm -h` // command usage
- `npm <command> -h`
- `npm help <command>` // documentation
- `npm help-search <command>`
- `npm api-help` // When using as an API

## package.json
- `npm init`
- `npm init -y`
- `npm set init-author-name "Bradley Flood"` // *-email*, *-url*, ++ see [docs](https://docs.npmjs.com/misc/config#init-author-name)
- `npm config set proxy="http://localhost:3127"`
- `npm set` === `npm config set` // || *npm get*
- `npm config delete proxy`
- `cat ~/.npmrc` // config settings
