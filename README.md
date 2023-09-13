# commitlint-config-traverson

shareable config for [commitlint](https://github.com/marionebl/commitlint)

<!--status-badges start -->

[![Node CI Workflow Status][github-actions-ci-badge]][github-actions-ci-link]
![SLSA Level 2][slsa-badge]

<!--status-badges end -->

## Purpose

This is a [shareable config](https://marionebl.github.io/commitlint/#/concepts-shareable-config) for [commitlint](https://github.com/marionebl/commitlint), which helps us ensure our commits are compatible with [semantic-release](https://github.com/semantic-release/semantic-release).

This config extends [commitlint-config-travi](https://github.com/travi/commitlint-config-travi).

## Usage

<!--consumer-badges start -->

[![npm][npm-badge]][npm-link]
[![MIT license][license-badge]][license-link]

<!--consumer-badges end -->

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

<!--contribution-badges start -->

[![Conventional Commits][commit-convention-badge]][commit-convention-link]
[![Commitizen friendly][commitizen-badge]][commitizen-link]
[![semantic-release][semantic-release-badge]][semantic-release-link]
[![PRs Welcome][PRs-badge]][PRs-link]
[![Renovate][renovate-badge]][renovate-link]

<!--contribution-badges end -->

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

[npm-badge]: https://img.shields.io/npm/v/commitlint-config-traverson?logo=npm

[license-link]: LICENSE

[license-badge]: https://img.shields.io/github/license/traverson/commitlint-config-traverson.svg

[commit-convention-link]: https://conventionalcommits.org

[commit-convention-badge]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg

[commitizen-link]: http://commitizen.github.io/cz-cli/

[commitizen-badge]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg

[semantic-release-link]: https://github.com/semantic-release/semantic-release

[semantic-release-badge]: https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release

[PRs-link]: http://makeapullrequest.com

[PRs-badge]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg

[github-actions-ci-link]: https://github.com/traverson/commitlint-config-traverson/actions?query=workflow%3A%22Node.js+CI%22+branch%3Amaster

[github-actions-ci-badge]: https://img.shields.io/github/actions/workflow/status/traverson/commitlint-config-traverson/node-ci.yml.svg?branch=master&logo=github

[renovate-link]: https://renovatebot.com

[renovate-badge]: https://img.shields.io/badge/renovate-enabled-brightgreen.svg?logo=renovatebot

[slsa-badge]: https://slsa.dev/images/gh-badge-level2.svg
