# UFES - The Ultimate Front-end Environment Setup

[UFES](https://github.com/AurelioDeRosa/UFES) is an opinionated front-end environment setup meant to help developers in writing better code by following current best practices and adopting the best tools the web community has to offer. The core principles of UFES are:

- **code standardization**
- **automation**
- **scalability**
- **manageability**
- **performance**

This setup is mostly based on the conventions and the technologies I use on a regular basis, and on my own workflow. However, I though it was nice to publish it in case other developers might find its use beneficial for them or their team.

## Setup description

The setup is based on the libraries, tools, and architecture described in the following sections.

### Automation

These are the tools used by UFES to perform various tasks (or used to scaffold UFES in first place):

- [Grunt](http://gruntjs.com/)
- [Yeoman](http://yeoman.io/)

### Dependency management

To manage the dependencies UFES uses:

- [npm](https://www.npmjs.com/)
- [Bower](http://bower.io/)

### CSS

UFES adopts the following tools and architecture to help in writing clean, standardized, managable, and scalable CSS code:

- [ITCSS](https://speakerdeck.com/dafed/managing-css-projects-with-itcss)
- [BEM](https://en.bem.info/)
- [SCSS](http://sass-lang.com/)
- [SCSS-Lint](https://github.com/brigade/scss-lint)
- [Autoprefixer](https://github.com/postcss/autoprefixer)
- [clean-css](https://github.com/jakubpawlowicz/clean-css)

### JavaScript

To help in writing clean, testable, managable, and scalable JavaScript code UFES relies on:

- [Browserify](http://browserify.org/)
- [JSCS](http://jscs.info/)
- [JSHint](http://jshint.com/)
- [Uglify](https://github.com/mishoo/UglifyJS2/)
- [jQuery](http://jquery.com/)
- [Modernizr](http://modernizr.com/)
- [Mocha](http://mochajs.org/)

### Images

The following tools are used to optimize the images:

- [jpegtran](https://github.com/kevva/imagemin-jpegtran)
- [optipng](https://github.com/kevva/imagemin-optipng)
- [gifsicle](https://github.com/kevva/imagemin-gifsicle)
- [svgo](https://github.com/kevva/imagemin-svgo)
- [spritesmith](https://github.com/Ensighten/spritesmith)

### UX

UFES uses the following libraries to improve the UX:

- [FastClick](https://github.com/ftlabs/fastclick)

## Style

The structure of the `style` folder follows the [ITCSS architecture](https://speakerdeck.com/dafed/managing-css-projects-with-itcss) proposed by [Harry Roberts](https://twitter.com/csswizardry) and described in [this talk](https://www.youtube.com/watch?v=1OKZOV-iLj4) and [this slide deck](https://speakerdeck.com/dafed/managing-css-projects-with-itcss). ITCSS proposes the use of the layers described below.

### settings

Contains global variables such as colors, fonts, and breakpoints used by the whole project.

### tools

Contains global mixins and functions used throughout the project.

### generic

Contains ground-zero styles such as Normalize.css and Reset.css.

### base

Contains the style of elements without specific classes like `blockquote`, `ul`, and `p`.

### objects

Contains objects that follow design patterns. This layer is particularly important if you're adhering to the OOCSS methodology.

### components

Contains designed components and chunks of UI.

### trumps

Contains helpers and overrides. The classes in this layer usually carry the `!important` declaration.

## License

UFES is dual licensed under the [MIT](http://www.opensource.org/licenses/MIT) and the [GPL-3.0](http://opensource.org/licenses/GPL-3.0) licenses.

## Author

[Aurelio De Rosa](http://www.audero.it) ([@AurelioDeRosa](https://twitter.com/AurelioDeRosa))