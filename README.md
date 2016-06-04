# eslint-config-redteal

[![npm](https://img.shields.io/npm/v/eslint-config-redteal.svg)][npm]

Redteal's ESLint 2.x config

## Install

```bash
npm install --save-dev eslint eslint-config-redteal
```

## Usage

We export two ESLint configs for your usage.

### eslint-config-redteal

Our default export extends Airbnb's rules, including ECMAScript 2015+,
with the tweaks below.

Add `"extends": "redteal"` to your .eslintrc

| Rule                   | airbnb-base | redteal |
|------------------------|-------------|---------|
| [global-require]       | error       | off     |
| [no-shadow]            | error       | off     |
| [no-underscore-dangle] | error       | off     |
| [sort-imports]         | off         | error   |

See [eslint-config-airbnb-base] and [Airbnb's styleguide] for more information.

### eslint-config-redteal/angular

Extends both the base config and [eslint-config-angular] to offer additional
rules for AngularJS development, with the tweaks below.

Add `"extends": "redteal/angular"` to your .eslintrc

| Rule                      | angular | redteal |
|---------------------------|---------|---------|
| angular/no-service-method | error   | off     |

See [eslint-config-angular] for more information.

[npm]: https://www.npmjs.com/package/eslint-config-redteal
[eslint-config-airbnb-base]: https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb-base
[Airbnb's styleguide]: https://github.com/airbnb/javascript
[global-require]: http://eslint.org/docs/rules/global-require
[no-shadow]: http://eslint.org/docs/rules/no-shadow
[no-underscore-dangle]: http://eslint.org/docs/rules/no-underscore-dangle
[sort-imports]: http://eslint.org/docs/rules/sort-imports
[eslint-config-angular]: https://github.com/dustinspecker/eslint-config-angular
