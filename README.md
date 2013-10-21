# jQuery CoffeeStain Plugin

A jQuery plugin to spoil your beautifully crafted website with a coffee mug stain.

## Getting Started

Download the [production version][min] or the [development version][max] of jQuery.coffeestain.

[min]: https://raw.github.com/robertprice/jquery-coffeestain/master/dist/jquery.coffeestain.min.js
[max]: https://raw.github.com/robertprice/jquery-coffeestain/master/dist/jquery.coffeestain.js

##  In the browser:

```
<script src="http://code.query.com/jquery.js"></script>
<script src="jquery.coffeestain.js"></script>
<script>
  $('myselector').coffeestain();
</script>
```

## Configuration Settings

```
$('myselector').coffeestain({
    // The top position of the coffee stain in the selected element
    top: 0,
    // The left position of the coffee stain in the selected element
    left: 0,
    // The opactity of the coffee stain
    opacity: 0.7,
    // The z-index of the coffee stain to ensure it sits on top of the other elements
    zIndex: 2000,
    // The image to use for the coffee stain, base64 encoded
    coffeeImg: "data:image/png;base64,iVBORw0KGgoAAAANS..."
});
```

## Bugs and Issues

The coffee stain is absolutely positioned with a high 'z-index' over the selected element.
To pass events such as clicks through to elements underneath, 'pointer-events' are used
but this is not supported in Internet Explorer. This means in IE, you may not be able to 
click through the stain to the elements below.

## Contributing

You are welcome to contribute to jQuery.coffeestain.js, install [grunt](https://github.com/cowboy/grunt) globally (```$ npm install grunt -g ```).

Do not edit files in the "dist" directory as they are generated via grunt. You'll find source code in the "src" subdirectory. Work inside of the src directory, and use grunt to concat/min/test/lint the code before making a pull request. Running ```$ grunt``` from the root of this project will do this for you.

## License

Copyright (c) 2013 Robert Price

This project is built with "Cowboy" Ben Alman's [Grunt](https://github.com/cowboy/grunt).

This project was originally based on the jQuery.bootstrap.

[MIT License](ttp://zenorocha.mit-license.org/)

## Author

* [Robert Price](http://github.com/robertprice)
