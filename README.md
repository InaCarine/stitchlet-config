# Stitchlet config

Shared configuration packages for projects.
Centralize and standardize TypeScript, ESLint, Stylelint, Prettier, and other development configs across all projects.

## Packages

- @stitchlet/typescript-config — TypeScript configs for apps and libraries
- @stitchlet/eslint-config — ESLint rules for consistent code quality
- @stitchlet/stylelint-config — Stylelint rules for CSS and styling

## Installation

Install the desired config package in your project:

```sh
pnpm add -D @stitchlet/eslint-config @stitchlet/typescript-config @stitchlet/stylelint-config
```

## Usage

ESLint

```js
// eslint.config.js
import eslintConfig from '@stitchlet/eslint-config';

export default {
  extends: [eslintConfig],
};
```

Typescript

```json
// tsconfig.json
{
  "extends": "@stitchlet/typescript-config/base.json"
}
```

Stylelint

```js
// stylelint.config.js
import stylelintConfig from '@stitchlet/stylelint-config';

export default {
  extends: [stylelintConfig],
};
```

## Contributing

Open issues or pull requests for improvements or new configs.
Keep configs modular and well-documented.

## License

MIT
