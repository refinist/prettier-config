# @refinist/prettier-config

[![npm](https://img.shields.io/npm/v/@refinist/prettier-config.svg?colorA=56b3b4&colorB=f7ba3e)](https://npmjs.com/package/@refinist/prettier-config)

Prettier config

## Features

- 📏 2 spaces (default)
- 🔚 Semicolons
- 🔤 Single quotes
- ❌ No trailing commas
- 🏹 Avoid arrow parentheses
- 🌐 Ignore HTML whitespace sensitivity
- 🚫 Ignore common files (`node_modules`, `dist`, `pnpm-lock.yaml`...)，refer to [#4708](https://github.com/prettier/prettier/issues/4708#issuecomment-1448705672)
- ⚡ Faster JS/TS parsing with [Oxc](https://github.com/nicolo-ribaudo/prettier/tree/nicolo/plugin-oxc/packages/plugin-oxc)
- 🎨 With Tailwind CSS plugin (optional)

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

### Basic

```json
// package.json
{
  "prettier": "@refinist/prettier-config"
}
```

Or in `prettier.config.js`:

```js
// prettier.config.js
import config from '@refinist/prettier-config';
/** @type {import('prettier').Config} */
export default {
  ...config

  /* your custom config */
};
```

### With Tailwind CSS

If you're using Tailwind CSS, use the variant with the plugin:

```json
// package.json
{
  "prettier": "@refinist/prettier-config/with-tailwindcss"
}
```

Or in `prettier.config.js`:

```js
// prettier.config.js
import config from '@refinist/prettier-config/with-tailwindcss';
/** @type {import('prettier').Config & import('@refinist/prettier-config/plugin-tailwindcss').PluginOptions} */
export default {
  ...config

  /* your custom config */
};
```

For more details about the Tailwind CSS plugin options, see the [prettier-plugin-tailwindcss documentation](https://github.com/tailwindlabs/prettier-plugin-tailwindcss).

Generally, prettier works together with eslint. Check out [@refinist/eslint-config](https://github.com/refinist/eslint-config?tab=readme-ov-file#-prettier-config) for more configuration details.

Inspired by [@sxzz](https://github.com/sxzz)

## License

[MIT](./LICENSE)

Copyright (c) 2025-present, Zhifeng (Jeff) Wang
