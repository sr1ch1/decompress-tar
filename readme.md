# decompress-tar [![Build Status](http://img.shields.io/travis/kevva/decompress-tar.svg?style=flat)](https://travis-ci.org/kevva/decompress-tar)

> tar decompress plugin


## Install

```
$ npm install --save decompress-tar
```


## Usage

```js
const decompress = require('decompress');
const decompressTar = require('decompress-tar');

decompress('unicorn.tar', 'dist', {
	plugins: [
		decompressTar()
	]
}).then(() => {
	console.log('Files decompressed');
});
```


## API

### decompressTar()(input)

Returns both a Promise for a Buffer and a [Duplex stream](https://nodejs.org/api/stream.html#stream_class_stream_duplex).

#### input

Type: `Buffer` `Stream`

Buffer or stream to decompress.


## License

MIT © [Kevin Mårtensson](https://github.com/kevva)
