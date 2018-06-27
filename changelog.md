# eslint-config-env changelog

## Next

- Updated dependencies.
- Support [Next.js](https://nextjs.org) projects.
- Fix React installation instructions.
- Throw an error if the `eslint` peer dependency is not a project dev dependency.
- New browser project setup:
  - Use [eslint-plugin-compat](https://npm.im/eslint-plugin-compat).
  - Automatically set `env.browser`.
- Only force modern ES syntax in a browser project if Babel is used.
- Next.js project improvements:
  - `parserOptions.sourceType` is `module`, as Next.js only supports ESM in `.js` files. Once Next.js updates to `webpack` >= 4 this will be reverted and `.mjs` should be used for ESM source files instead.
  - Disabled the [`react/react-in-jsx-scope` rule](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/react-in-jsx-scope.md), as Next.js uses [`babel-plugin-react-require`](https://npm.im/babel-plugin-react-require).

## 0.3.0

- Updated dependencies.

## 0.2.0

- Updated dependencies.
- Updated preferred JSDoc tag synonyms:
  - `@param`
  - `@prop`
  - `@returns`

## 0.1.1

- Fix a crash when a package is missing `peerDependencies`, `dependencies` or `devDependencies` fields.

## 0.1.0

- Initial release.
