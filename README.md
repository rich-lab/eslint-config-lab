# ESLint config for 🍷Lab🍷

This config is supposed to work with [XO](https://github.com/sindresorhus/xo) or [eslint-config-xo](https://github.com/sindresorhus/eslint-config-xo).

## Features

- Indent with 2 spaces and no semicolon
- [Lint code blocks in Markdown!](#lint-code-blocks-in-markdown)
- [Enforce consistent spacing inside](https://eslint.org/docs/rules/object-curly-spacing)
- [Require Following Curly Brace Conventions with `multi` option](https://eslint.org/docs/rules/curly#multi)
- [Disallow unused expressions](https://eslint.org/docs/rules/no-unused-expressions)

## Install

```bash
yarn add -D eslint-config-lab
# OR: npm install -D eslint eslint-config-lab
```

## Usage

In ESLint:

```js
/* package.json */
{
  "eslintConfig": {
    "extends": ["xo/esnext", "lab"]
  }
}
```

Or in XO:

```js
/* package.json */
{
  "xo": {
    "extends": "lab"
  }
}
```

### Lint code blocks in markdown

It uses [eslint-plugin-markdown](https://github.com/eslint/eslint-plugin-markdown):

```json
{
  "xo": {
    "extensions": ["md"]
  }
}
```

## License

[MIT](./LICENSE)

Copyright (c) 2018-present, ULIVZ & SHERRY
