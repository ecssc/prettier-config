# @ecssc/prettier-config

Shared Prettier configuration for ECSSC projects.

## Installation

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