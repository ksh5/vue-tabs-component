**COMPONENT IN DEVELOPMENT: DO NOT USE YET**

# A Vue component to easily render tabs

[![Latest Version on NPM](https://img.shields.io/npm/v/vue-tabs.svg?style=flat-square)](https://npmjs.com/package/vue-tabs)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)
[![Build Status](https://img.shields.io/travis/spatie/vue-tabs/master.svg?style=flat-square)](https://travis-ci.org/spatie/vue-tabs)

The package contains Vue components to easily display some tabs.

This is how they can be used:

```html
<div>
    <tabs>
        <tab name="First tab">
            First tab content
        </tab>
        <tab name="Second tab">
            Second tab content
        </tab>
        <tab name="Third tab">
            Third tab content
        </tab>
    </tabs>
</div>
```

[Here's a demo](TO DO: add link) that shows how that content could look like.

## Postcardware

You're free to use this package (it's [MIT-licensed](LICENSE.md)), but if it makes it to your production environment we highly appreciate you sending us a postcard from your hometown, mentioning which of our package(s) you are using.

Our address is: Spatie, Samberstraat 69D, 2060 Antwerp, Belgium.

All postcards are published [on our website](https://spatie.be/opensource/postcards).

## Install

You can install the package via yarn:

```bash
$ yarn add @spatie/vue-tabs
```

## Usage

The most common use case is to register the component globally

```js
//in your app.js or similar file
import Vue from 'vue';
import {tabs, tab} from 'vue-tabs';

Vue.component('tabs', Tabs);
Vue.component('tab', Tab);
```

On your page you can now use html like this to render tabs: 

```html
<div>
    <tabs>
        <tab name="First tab">
            First tab content
        </tab>
        <tab name="Second tab">
            Second tab content
        </tab>
        <tab name="Third tab">
            Third tab content
        </tab>
    </tabs>
</div>
```

### Customizing fragments

When clicking on a tab it's name will be used as a fragment in the url. For example clicking on the `Second tab` will append `#second-tab` to the current url. 

You can customize that fragment by using the `href` attribute.

```html
<div>
    <tabs>
        <tab name="My tab" href="custom-href">
            First tab content
        </tab>
    </tabs>
</div>
```

Clicking on `My tab` will then append `#custom-href` to the url.

## Change log

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Testing

``` bash
$ yarn run test
```

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Security

If you discover any security related issues, please contact [Freek Van der Herten](https://github.com/freekmurze) instead of using the issue tracker.

## Credits

- [Freek Van der Herten](https://github.com/freekmurze)
- [All Contributors](../../contributors)

This package is heavily based on the solution presented by Jeffrey Way in the [practical example #3](https://laracasts.com/series/learn-vue-2-step-by-step/episodes/11) video in the [Vue series](https://vuecasts.com) on [Laracasts](https://laracasts.com)

## About Spatie
Spatie is a webdesign agency based in Antwerp, Belgium. You'll find an overview of all our open source projects [on our website](https://spatie.be/opensource).

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
