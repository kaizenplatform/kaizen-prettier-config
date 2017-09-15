# @kaizenplatform/prettier-config

## Usage

Import config from `@kaizenplatform/prettier-config` in your `prettier.config.js`

```js
module.exports = require('@kaizenplatform/prettier-config');
```

Customizing use-case:

```js
const defaultOptions = require('@kaizenplatform/prettier-config');

module.exports = Object.assign({}, defaultOptions, {
    semi: false,
    overrides: [
        {
            files: '*.test.js',
            options: {
                semi: true,
            },
        },
    ],
});
```

## Developing

The definition of prettier options is in `index.js`. You can send PR to edit it.

**Every option which is different to default should have its reasons.**
