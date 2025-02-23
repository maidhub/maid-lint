<a name="readme-top"></a><div align="center">

<h1>Maid Lint</h1>

ESlint config, Prettier config, Remark config for MaidHub

[Changelog](./CHANGELOG.md)

</div>

![](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<details>
<summary><kbd>Table of contents</kbd></summary>

#### TOC

- [📦 Installation](#-installation)
- [🤯 Usage](#-usage)
  - [.npmrc](#npmrc)
  - [ESlint](#eslint)
  - [Stylelint](#stylelint)
  - [Commitlint](#commitlint)
  - [Changelog](#changelog)
  - [Remark](#remark)
  - [Prettier](#prettier)
  - [Semantic Release](#semantic-release)
- [⌨️ Local Development](#️-local-development)

####

</details>

## 📦 Installation

To install Maid Lint, run the following command:

```bash
$ bun add @maidhub/lint -D
```

To use template ignore files, run the following command:

```bash
$ curl -O https://raw.githubusercontent.com/maidhub/maid-lint/master/.eslintignore
$ curl -O https://raw.githubusercontent.com/maidhub/maid-lint/master/.gitignore
$ curl -O https://raw.githubusercontent.com/maidhub/maid-lint/master/.prettierignore
```

<div align="right">

</div>

## 🤯 Usage

### .npmrc

```text
public-hoist-pattern[]=*@umijs/lint*
public-hoist-pattern[]=*changelog*
public-hoist-pattern[]=*commitlint*
public-hoist-pattern[]=*eslint*
public-hoist-pattern[]=*postcss*
public-hoist-pattern[]=*prettier*
public-hoist-pattern[]=*remark*
public-hoist-pattern[]=*semantic-release*
public-hoist-pattern[]=*stylelint*
```

### ESlint

config can be found at [`.eslintrc.js`](/src/eslint/index.ts)

```js
module.exports = require('@maidhub/lint').eslint;
```

### Stylelint

config can be found at [`.stylelintrc.js`](/src/stylelint/index.ts)

```js
module.exports = require('@maidhub/lint').stylelint;
```

### Commitlint

config can be found at [`.commitlintrc.js`](/src/commitlint/index.ts)

```js
module.exports = require('@maidhub/lint').commitlint;
```

### Changelog

config can be found at [`.changelogrc.js`](/src/changelog/index.ts)

```js
module.exports = require('@maidhub/lint').changelog;
```

### Remark

config can be found at [`.remarkrc.js`](/src/remarklint/index.ts)

```js
module.exports = require('@maidhub/lint').remarklint;
```

### Prettier

config can be found at [`.prettierrc.js`](/src/prettier/index.ts)

```js
module.exports = require('@maidhub/lint').prettier;
```

### Semantic Release

config can be found at [`.releaserc.js`](/src/semantic-release/index.ts)

```js
module.exports = require('@maidhub/lint').semanticRelease;
```

<div align="right">

</div>

## ⌨️ Local Development

You can use Github Codespaces for online development:

Or clone it for local development:

```bash
$ git clone https://github.com/maidhub/maid-lint.git
$ cd maidhub/lint
$ bun install
$ bun start
```
