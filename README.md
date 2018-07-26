# commitlint-config-traverson

shareable config for [commitlint](https://github.com/marionebl/commitlint)

<!-- status badges -->
[![Build Status][ci-badge]][ci-link]

## Purpose

This is a [shareable config](https://marionebl.github.io/commitlint/#/concepts-shareable-config) for [commitlint](https://github.com/marionebl/commitlint), which helps us ensure our commits are compatible with [semantic-release](https://github.com/semantic-release/semantic-release).

This config extends [commitlint-config-travi](https://github.com/travi/commitlint-config-travi).

## Usage

<!-- consumer badges -->
[![npm][npm-badge]][npm-link]
[![MIT license][license-badge]][license-link]

### Installation

```sh
$ npm install commitlint-config-traverson --save-dev
```

### Define the config for your project

```sh
$ echo "module.exports = {extends: ['traverson']};" > .commitlintrc.js
```

### Define the [husky](https://github.com/typicode/husky) hook

([in a `.huskyrc.json`](https://github.com/typicode/husky#upgrading-from-014),
for example)

```json
{
  "hooks": {
    "commit-msg": "commitlint -e"
  }
}
```

## Contributing

<!-- contribution badges -->
[![Conventional Commits][commit-convention-badge]][commit-convention-link]
[![Commitizen friendly][commitizen-badge]][commitizen-link]
[![semantic-release][semantic-release-badge]][semantic-release-link]
[![PRs Welcome][PRs-badge]][PRs-link]

### Dependencies

```sh
$ nvm install
$ npm install
```

### Verification

```sh
$ npm test
```

[npm-link]: https://www.npmjs.com/package/commitlint-config-traverson
[npm-badge]: https://img.shields.io/npm/v/commitlint-config-traverson.svg
[license-link]: LICENSE
[license-badge]: https://img.shields.io/github/license/traverson/commitlint-config-traverson.svg
[ci-link]: https://travis-ci.com/traverson/commitlint-config-traverson
[ci-badge]: https://img.shields.io/travis/traverson/commitlint-config-traverson.svg?branch=master
[commit-convention-link]: https://conventionalcommits.org
[commit-convention-badge]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg
[commitizen-link]: http://commitizen.github.io/cz-cli/
[commitizen-badge]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
[semantic-release-link]: https://github.com/semantic-release/semantic-release
[semantic-release-badge]: https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg
[PRs-link]: http://makeapullrequest.com
[PRs-badge]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg
