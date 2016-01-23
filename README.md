gulp-jsx-docco
=============

[![NPM version]]

> docco plugin for [gulp](https://github.com/wearefractal/gulp)

JSX support added
-------------
This module added jsx support to gulp-docco(https://github.com/jsBoot/gulp-docco)
-------------

Install `gulp-jsx-docco` as a development dependency:

```shell
npm install --save-dev gulp-jsx-docco
```

Then, add it to your `gulpfile.js`:

```javascript
var docco = require("gulp-jsx-docco");

gulp.src("./src/*.js")
  .pipe(docco())
  .pipe(gulp.dest('./documentation-output'))
```

That's it.

## API

### options

Additionally, we support passing an options object following the [docco syntax](http://jashkenas.github.io/docco/):

```javascript
var docco = require("gulp-jsx-docco");

gulp.src("./src/*.js")
  .pipe(docco(options))
  .pipe(gulp.dest('./documentation-output'))
```

Mainly of interest are the various embedded layouts (parallel, linear, classic), and custom template support.

## Caveats?

We bypass some of docco internals in order to prevent it from manipulating files on its own - if something is broken, say so!

## License

[MIT License](http://en.wikipedia.org/wiki/MIT_License)

[npm-url]: https://npmjs.org/package/gulp-jsx-docco
