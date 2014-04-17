*This repository is a mirror of the [component](http://component.io) module [sindresorhus/pretty-ms](http://github.com/sindresorhus/pretty-ms). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/sindresorhus-pretty-ms`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# pretty-ms [![Build Status](https://travis-ci.org/sindresorhus/pretty-ms.svg?branch=master)](https://travis-ci.org/sindresorhus/pretty-ms)

> Convert milliseconds to a human readable string: `1337000000` ➔ `15d 11h 23m 20s`


## Install

```bash
$ npm install --save pretty-ms
```

```bash
$ bower install --save pretty-ms
```

```bash
$ component install sindresorhus/pretty-ms
```


## Usage

```js
prettyMs(1337000000);
//=> '15d 11h 23m 20s'

prettyMs(1337);
//=> '1.3s'

prettyMs(133);
//=> '133ms'

// compact option
prettyMs(1337, {compact: true});
//=> '~1s'

// can be useful for time durations
prettyMs(new Date(2014, 0, 1, 10, 40) - new Date(2014, 0, 1, 10, 5))
//=> '35m'
```


## API

### prettyMs(milliseconds, options)

#### milliseconds

*Required*  
Type: `number`

#### options.compact

Type: `boolean`

Only show the first unit: `1h 10m` ➔ `~1h`.


## CLI

```bash
$ npm install --global pretty-ms
```

```bash
$ pretty-ms --help

Usage
  $ pretty-ms <milliseconds> [--compact]
  $ echo <milliseconds> | pretty-ms

Example
  $ pretty-ms 1337
  1.3s
```


## License

[MIT](http://opensource.org/licenses/MIT) © [Sindre Sorhus](http://sindresorhus.com)
