[![NPM version](https://badge.fury.io/js/tslint-i18n.svg)](https://www.npmjs.com/package/tslint-i18n)
[![Downloads](http://img.shields.io/npm/dm/tslint-i18n.svg)](https://npmjs.org/package/tslint-i18n)
[![Circle CI](https://circleci.com/gh/hsuehic/tslint-i18n.svg?style=svg)](https://circleci.com/gh/hsuehic/tslint-i18n)

tslint-i18n
------------


Lint rules related to i18n for [TSLint](https://github.com/hsuehic/tslint/).

### Thanks
Code is based on https://github.com/palantir/tslint-react. Thanks to the authors.

### Usage

tslint-i18n has peer dependencies on TSLint and TypeScript.

To use these lint rules with the default preset, use configuration inheritance via the `extends` keyword.
Here's a sample configuration where `tslint.json` lives adjacent to your `node_modules` folder:

```js
{
  "extends": ["tslint:latest", "tslint-i18n"],
  "rules": {
    // override tslint-i18n rules here
    "i18n-no-literal": false
  }
}
```

To lint your `.ts` **and** `.tsx` files you can simply run `tslint -c tslint.json 'src/**/*.{ts,tsx}'`.

### Semantic versioning

The built-in configuration preset you get with `"extends": "tslint-i18n"` is semantically versioned in a manner similar to TSLint's built-in presets and the TypeScript language itself. As new rules are added to tslint-i18n across minor versions, stricter checks may be enabled here. Your code is not guaranteed to continue passing checks across these version bumps. If you wish to ensure that `npm upgrade` or `yarn upgrade` never breaks your build, declare a tilde dependency on this package (e.g. `"~1.0.0"`).

### Rules


### Development

We track rule suggestions on Github issues -- [here's a useful link](https://github.com/hsuehic/tslint-i18n/issues?q=is%3Aissue+is%3Aopen+label%3A%22Type%3A+Rule+Suggestion%22)
to view all the current suggestions. Tickets are roughly triaged by priority (P1, P2, P3).

We're happy to accept PRs for new rules, especially those marked as [Status: Accepting PRs](https://github.com/hsuehic/tslint-i18n/issues?q=is%3Aissue+is%3Aopen+label%3A%22Status%3A+Accepting+PRs%22).
If submitting a PR, try to follow the same style conventions as the [core TSLint project](https://github.com/hsuehic/tslint).

Quick Start (requires Node v6+, yarn v0.22+):

1. `yarn`
1. `yarn verify`
1. `yarn lint`

### Changelog

See the Github [release history](https://github.com/hsuehic/tslint-i18n/releases).
