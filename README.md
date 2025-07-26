# @refinist/prettier-config [![npm](https://img.shields.io/npm/v/@refinist/prettier-config.svg?colorA=56b3b4&colorB=f7ba3e)](https://npmjs.com/package/@refinist/prettier-config)

Prettier config

## Install

Using pnpm, yarn, or npm

```bash
# with pnpm
pnpm add -D @refinist/prettier-config

# with yarn
yarn add -D @refinist/prettier-config

# with npm
npm i -D @refinist/prettier-config
```

## Usage

```json
// package.json
{
  "prettier": "@refinist/prettier-config"
}
```

Generally, prettier works together with eslint. Check out [@refinist/eslint-config](https://github.com/refinist/eslint-config?tab=readme-ov-file#-prettier-config) for more configuration details.

## Features

- 📏 2 spaces (default)
- 🔚 Semicolons
- 🔤 Single quotes
- ❌ No trailing commas
- 🏹 Avoid arrow parentheses
- 🌐 Ignore HTML whitespace sensitivity
- 🚫 Ignore common files (`node_modules`, `dist`, `pnpm-lock.yaml`...)，refer to [#4708](https://github.com/prettier/prettier/issues/4708#issuecomment-1448705672)

Inspired by [@sxzz](https://github.com/sxzz)

## License

[MIT](./LICENSE)

Copyright (c) 2025-present, Zhifeng (Jeff) Wang
