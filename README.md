[medium-editor](https://github.com/yabwe/medium-editor) library for Ember Apps.

Compatibility
------------------------------------------------------------------------------

* Ember.js v3.4 or above
* Ember CLI v2.13 or above
* Node.js v8 or above


Installation
------------------------------------------------------------------------------

```
ember install my-addon
```
>>>>>>> 4700837... message

## Installation

With `ember`:

* `ember install ember-medium-editor`

With `npm`:

* `npm install --save-dev ember-medium-editor`

## Configuration

```js
// ember-cli-build.js
let app = new EmberApp(defaults, {
  mediumEditor: {
    /**
    * If true will include only JS in the build.
    *
    * @type Boolean
    * @default false
    */
    excludeStyles: false,
    
    /**
    * List of themes: https://github.com/yabwe/medium-editor/tree/master/dist/css/themes
    *
    * @type String
    * @default 'default'
    */
    theme: 'default'
  }
});
```

## Usage

```handlebars
{{medium-editor
    model.text
    options=(hash)
    onChange=(action (mut model.text))}}
```

## Issues

If you encounter any issue please report it [here](https://github.com/kolybasov/ember-medium-editor/issues).

## Licence

[MIT](./LICENSE.md)
