# Ractive.js bacon adaptor plugin

*Find more Ractive.js plugins at [docs.ractivejs.org/latest/plugins](http://docs.ractivejs.org/latest/plugins)*

[See the demo here.](http://ractivejs.github.io/ractive-adaptors-bacon)

## Usage

Include this file on your page below Ractive, e.g:

```html
<script src='lib/ractive.js'></script>
<script src='lib/ractive-adaptors-bacon.js'></script>
```

Or, if you're using a module loader, require this module:

```js
// requiring the plugin will 'activate' it - no need to use the return value
require( 'ractive-adaptors-bacon' );
```

Then, tell Ractive to use the `Bacon` adaptor:

```js
ractive = new Ractive({
  el: 'body',
  template: myTemplate,
  adapt: 'Bacon',
  data: {
    foo: someReactiveProperty
  }
});
```


## Notes

This is a work-in-progress! In particular, two-way binding is not yet implemented.



## License

Copyright (c) 2014 Rich Harris. Licensed MIT

Created with the [Ractive.js plugin template](https://github.com/ractivejs/plugin-template) for Grunt.
