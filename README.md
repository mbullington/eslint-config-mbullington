# eslint-config-mbullington

"Just works" ESLint/Prettier config for personal projects.

Continuation of `@dji-dev/us-web-config`, an [open-source](https://github.com/dji-dev/us-web) project I authored while at DJI Research LLC.

## Installing

`yarn add -D eslint-config-mbullington`

Using `yarn` is highly recommended but not required.

# Linting Features

`yarn add --dev eslint @babel/core`

If using TypeScript also do:

`yarn add --dev typescript`

If using GraphQL also do:

`yarn add graphql`

For ESLint, create an `.eslintrc.js` file that has the following:

```js
module.exports = require('eslint-config-mbullington')({
    typescript: true,
    graphql: false,
    react: true,
    vue: false,
})
```

(update the fields accordingly for your project.)

# VSCode

If using VSCode, for easy results you can copy this into `.vscode/settings.json` of project:

```json
{
    "eslint.enable": true,
    "eslint.validate": ["javascript", "javascriptreact", "typescript", "typescriptreact", "vue"],
    "editor.tabSize": 4
}
```

Make sure the official `ESLint` plugin is installed.