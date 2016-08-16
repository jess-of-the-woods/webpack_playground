# webpack_playground
A repo to play with learning Webpack


Bit confused about why I need to rename the require in app.js to `require('./logger.es6')
`. According to the article, the resolve key:

```javascript
resolve: {
  extensions: ['', '.js', '.es6']
}
```
in webpack.config.js should mean it will work without needing to rename.


---
Also getting this message when running `webpack --config webpack-production.config.js -p`:

```
ERROR in bundle.js from UglifyJs
SyntaxError: Unexpected token: name (checkName) [./~/strip-loader/lib?strip[]=console.log!./~/jshint-loader!./logger.es6.js:3,0]
```

Doesn't happen without `-p` (production(minify)) flag

---

Based on the Beginner's guide to Webpack [tutorial](https://medium.com/@dabit3/beginner-s-guide-to-webpack-b1f1a3638460#.anh3ggrrl) | [repo](https://github.com/dabit3/beginning-webpack)
