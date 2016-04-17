# Horizon React-Native Example Application
This is an example application which shows how to set up [horizon](https://github.com/rethinkdb/horizon) with [react-native](https://facebook.github.io/react-native/).

## Preparing development

Install global packages if you don't have them already

```bash
$ npm install -g react-native-cli
$ npm install -g horizon
```


Install local dependencies
```bash
$ cd HorizonExampleApp
$ npm install
```

## Starting development

Starting bundler & simulator
```bash
$ cd HorizonExampleApp
$ npm start
$ react-native run-ios # in a new terminal instance
```

Staring Horizon server
```bash
$ cd server
$ hz serve --dev
```


## How is this set up?
These steps were executed to set up this project:

```bash
$ mkdir horizon-react-native
$ cd horizon-react-native

$ npm i -g react-native-cli # if you don't have it already

# create react-native application
$ react-native init HorizonExampleApp

# now on to horizon
$ hz init server
$ cd server
$ rm -r dist src # remove unused directories
```

Finally, some horizon code was added to `HorizonExampleApp/index.ios.js`.


You could go from here for real projects and set up proper npm scripts,
get rid of the global dependencies and so on.
