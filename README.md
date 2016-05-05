# NPM cheat sheet

> SASS Compiler <a href="https://www.npmjs.com/package/sass">[LINK]</a>

`$ [sudo] gem install sass`

`$ cd floating-space-man`

First run `$ touch styles.scss styles.css`

`$ sass --watch styles.scss:styles.css --style compressed` compressed will minify on un-watch

When done:

`Ctrl+C` via Terminal to exit watch

> UglifyJS 2 Compress, Scramble, Beautify <a href="https://github.com/mishoo/UglifyJS2">[LINK]</a>

`$ [sudo] npm install uglify-js -g`

To uncompress `main.min.js`

`$ uglifyjs main.min.js -b -o main.js`

To compress & mangle `main.js`

`$ uglifyjs main.js -c -m -o main.min.js`

> PurifyCSS A function that takes content (HTML/JS/PHP/etc) and CSS, and returns only the used CSS <a href="https://github.com/purifycss/purifycss">[LINK]</a>

`$ [sudo] npm install -g purify-css`

`$ purifycss <css-file-to-purify> <html/js/php-file-to-compare-to> --info --out <output-css-file>`

`$ pufifycss styles.scss index.html --info --out styles-new.scss`

> BeautifyCSS A command-line CSS beautifier <a href="https://www.npmjs.com/package/beautify-css">[LINK]</a>

`$ beautify-css [options] [input] [output]`

`$ beautify-css -p styles.scss` - will overwrite existing file (dev)

`$ beautify-css styles.scss styles-new.scss` - will create new file (dev)

`$ beautify-css -p -c styles.scss` - will overwrite & compress (prod)
