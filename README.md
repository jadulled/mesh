# Mesh v.4.0.0

Mesh is a responsive, mobile first fluid grid system, built on LESS, for easy customization.

## Development setup
- Clone
- Run `npm install && bower install` in the command line to install project dependencies.
- Run `gulp` to build dist files. 
- Run `gulp watch` to create a server in node and run the demo in the browser.

## Use guide

By default mesh uses a 12 column grid system: it divides the space available by 12.

To give your columns the desired width use the class `.mesh-` + the number of columns out of 12 you want this element to measure. The columns must add 12 for them to cover the whole space available. By defualt mesh generates a gutter of 30px bretween columns.

For example you can have `<div class="mesh-3"></div>` next to a `<div class="mesh-9"></div>` element to have a layout with a narrow side-bar and a wide main conetent area. Between both they add up twelve.

You can also have a more complex responsive layout where in mobile your columns use all the space available of the container and stack up one below the other, but from tablets up they split to be next to each other. In this case you may have to use a `<div class="mesh-xs-12 mesh-s-4"></div>` next to a `<div class="mesh-xs-12 mesh-s-8"></div>`.

You can use as many elements in your container but they must add up to 12 so you do not have empty spaces in your grid.

The available classes to target different screen resolutions are:

- `.mesh-xs-` Phone devices and up.
- `.mesh-s-` Targets tablet devices and up.
- `.mesh-m-` Targets landscape tablets and small dektops and up.
- `.mesh-l-` Targets desktops 1200px and up.

Basic class:
- `.mesh-` Is device agnostic, uses the same width proportion through all devices and resolutions.

It is <strong>recommended</strong> to wrap your grids in a `.row` element. This helper clears the floats and resets the left gutter from the first element and the right gutter from the last one.

## Options

In the variables.less file you can customize mesh. Change the breakpoints, set the total number of columns if you disslike 12, and change the gutter size.
After changing the settings don't forget to re-build the component running the `gulp` command, the css files are compiled in the dist folder ready to be used in your personal project.

**NOTE**

Please read through our code style guides:
- [HTML](https://github.com/mercadolibre/html-style-guide)
- [CSS](https://github.com/mercadolibre/css-style-guide)


## Maintained by

- Her Mammana ([@hmammana](https://twitter.com/hmammana))
- Lean Linares ([@lean8086](https://twitter.com/lean8086))
- Guille Paz ([@pazguille](https://twitter.com/pazguille))
- Nati Devalle ([@taly](https://twitter.com/taly))
- Juan Vanni ([@jota_v_](https://twitter.com/jota_v_))


## Credits

![MercadoLibre](http://static.mlstatic.com/org-img/chico/img/logo-mercadolibre-new.png)

## License
Licensed under the MIT license.

Copyright (c) 2013 [MercadoLibre](http://github.com/mercadolibre).
