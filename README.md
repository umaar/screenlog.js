screenlog.js
=====
*console.log, but on the screen*
***

Ever faced a situation where you said "Why doesn't this bug show up when developer console is open!!"? And since the bug doesn't show when you have console open, you cannot do debug logging using `console.log`.

Enter `screenlog.js`. `screenlog.js` brings the developer console right on your screen so that you can do logging without having the developer console open always.

### [DEMO](http://kushagragour.in/lab/ctajs)

Installation
-----

`npm install screenlog`

Drop `screenlog.js` into your web application and initialize it with:

```js
screenLog.init();
```

And you are done! By default, every `console.log` in your now starts logging on the screen.


Public API
-----

### screenLog.init([options])

Animate an element `sourceElement` onto `targetElement`.

* `options` - A map of additional options to control the animation behaviour.
	* `color` - Text color. Default is `lightgreen`.
	* `bgColor` - Background color of the log panel. Default is `black`.
	* `releaseConsole` - By default console.log is overridden to log on screen. You can avoid this behaviour by setting `releaseConsole` to `true` and instead use `screenLog.log()` api. Default is `false`.

### screenLog.log(obj1 [, obj2, ..., objN])

Logs a message on the screen.

* `obj1 ... objN` - A list of JavaScript objects or strings to output. Just like `console.log`.

### screenLog.clear()

Clear messages on the screen.

Browser Support
-----

**screenlog.js** works best on latest versions of Google Chrome, Firefox and Safari.

Contributing
-----

Interested in contributing features and fixes?

[Read more on contributing](./CONTRIBUTING.md).

Changelog
-----

See the [Changelog](https://github.com/chinchang/screenlog.js/wiki/Changelog)

License
-----

Copyright (c) 2015 Kushagra Gour, http://kushagragour.in
Licensed under the [MIT license](http://opensource.org/licenses/MIT).
