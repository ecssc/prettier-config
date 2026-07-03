# @ecssc/prettier-config

Shared Prettier configuration for ECSSC projects. Requires Prettier 3+.

## Installation

These packages are published to GitHub Packages. Add an `.npmrc` to your project pointing the `@ecssc` scope at that registry:

```
@ecssc:registry=https://npm.pkg.github.com
//npm.pkg.github.com/:_authToken=${NODE_AUTH_TOKEN}
```

GitHub Packages requires authentication even for public packages, so `NODE_AUTH_TOKEN` must hold a token with the `read:packages` scope. Then install:

```bash
npm install --save-dev @ecssc/prettier-config prettier
```

## Usage

Add to your `package.json`:

```json
{
  "prettier": "@ecssc/prettier-config"
}
```

Or create a `.prettierrc.mjs`:

```javascript
export { default } from '@ecssc/prettier-config'
```

## Configuration

- Print width: 90
- No semicolons
- Single quotes
- Trailing commas (ES5)
- Tailwind CSS class sorting via `prettier-plugin-tailwindcss`