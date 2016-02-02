Web Boilerplate
===

A bunch of `npm scripts` plumbing on top of

* Bundling and minifcation of JS ([browserify](http://browserify.org))
* ES6 transpilation with [babel](https://babeljs.io/)
* Base CSS incl. imports with [postcss-cssnext](http://cssnext.io/) and [normalize.css](https://necolas.github.io/normalize.css/)
* Compresses images using [imagemin](https://github.com/imagemin/imagemin)
* Hashes css, js and images for effective caching ([hashmark](https://github.com/keithamus/hashmark))
* File watching during development ([watchify](https://github.com/substack/watchify), [postcss-cli](https://github.com/postcss/postcss-cli))

## Installation

Download this project and run:
```
npm install
```

or use this one-liner:

```
mkdir web-boilerplate && cd web-boilerplate && curl -L# https://github.com/klaemo/web-boilerplate/archive/master.zip | tar xz --strip 1 && npm install
```

## Development

Starts server, watches JS and CSS
```
npm run dev
```

## Production build

* Bundles, transpiles and minifies JS
* Bundles, post-processes and minifies CSS.
* Optimizes images.
* Appends hash to filenames for reliable cache busting.
* Replaces references to images in CSS with hashed version (e.g. `/img/image.png` -> `/img/image.0dedbaee.png`).

Everything ends up in `public` and is ready to be deployed somewhere

```
npm run compile
```

## License
MIT
