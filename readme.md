# tachyons-background-size 3.0.3

Background size CSS module for Tachyons

#### Stats

310 | 8 | 8
---|---|---
bytes | selectors | declarations

## Installation

#### With [npm](https://npmjs.com)

```
npm install --save-dev tachyons-background-size
```

#### With Git

```
git clone https://github.com/tachyons-css/tachyons-background-size
```

## Usage

#### Using with [PostCSS](https://github.com/postcss/postcss)

Import the css module

```css
@import "tachyons-background-size";
```

Then process the CSS using the [`tachyons-cli`](https://github.com/tachyons-css/tachyons-cli)

```sh
$ npm i -g tachyons-cli
$ tachyons-cli path/to/css-file.css > dist/t.css
```

#### Using the CSS

The built CSS is located in the `css` directory. It contains an unminified and minified version.
You can either cut and paste that css or link to it directly in your html.

```html
<link rel="stylesheet" href="path/to/module/css/tachyons-background-size">
```

#### Development

The source CSS files can be found in the `src` directory.
Running `$ npm start` will process the source CSS and place the built CSS in the `css` directory.

## The CSS

```css
/*

   BACKGROUND SIZE

   Base:
    bg = background-size

   Modifiers:
    -cv = cover
    -cn = contain

   Media Query Extensions:
     -ns = not-small
     -m  = medium
     -l  = large

*/
/*
  Often used in combination with background image set as an inline style
  on an html element.
*/
.bg-cv { background-size: cover; }
.bg-cn { background-size: contain; }
@media screen and (min-width: 48em) {
 .bg-cv-ns { background-size: cover; }
 .bg-cn-ns { background-size: contain; }
}
@media screen and (min-width: 48em) and (max-width: 64em) {
 .bg-cv-m { background-size: cover; }
 .bg-cn-m { background-size: contain; }
}
@media screen and (min-width: 64em) {
 .bg-cv-l { background-size: cover; }
 .bg-cn-l { background-size: contain; }
}
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## Authors

* [mrmrs](http://mrmrs.io)
* [johno](http://johnotander.com)

## License

MIT

