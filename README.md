# eslint-config-auz [![Build Status](https://travis-ci.org/auzmartist/eslint-config-auz.svg?branch=master)] [![npm version](https://badge.fury.io/js/eslint-config-auz.svg)](https://badge.fury.io/js/eslint-config-auz)

> ESLint [shareable config](http://eslint.org/docs/developer-guide/shareable-configs.html) for the [Google JavaScript style guide on which this is based](https://google.github.io/styleguide/jsguide.html)

## Usage

Once the `eslint-config-auz` package is installed, you can use it by specifying `auz` in the [`extends`](http://eslint.org/docs/user-guide/configuring#extending-configuration-files) section of your [ESLint configuration](http://eslint.org/docs/user-guide/configuring).

```js
{
	"extends": "auz",
	"rules": {
		// Additional, per-project rules...
	}
}
```

### Using the `auz` config with `eslint:recommended`

There are several rules in the [`eslint:recommended` ruleset](http://eslint.org/docs/rules/) that this style is not opinionated about that you might want to enforce in your project.

To use this style in conjunction with ESLint's recommended rule set, extend them both, making sure to list `auz` last:

```js
{
	"extends": ["eslint:recommended", "auz"],
	"rules": {
		// Additional, per-project rules...
	}
}
```

To see how the `auz` config compares with `eslint:recommended`, refer to the [source code of `index.js`](https://github.com/auzmartist/eslint-config-auz/blob/master/index.js), which lists every ESLint rule along with whether (and how) it is enforced by the `auz` config. For more on how the Google style differs from this fork, visit the [eslint-config-google repository.](https://github.com/google/eslint-config-google/)


## License

Apache-2
