# prettier-config
A personal, shareable [Prettier](https://prettier.io/) configuration.

## Usage

Install the package using a package manager of your choice:

```sh
// npm
npm install --save-dev @patricktabar/prettier-config

// yarn
yarn add -D @patricktabar/prettier-config

// pnpm
pnpm add -D @patricktabar/prettier-config
```

Add the `prettier` key to your `package.json`

```diff
+  "prettier": "@github/prettier-config",
 ```
 
 or extend the `.prettierrc` file to override some properties from the shared configuration:

```js
import prettierConfig from "@patricktabar/prettier-config";

export default {
  ...prettierConfig,
  semi: false,
};
```

 [Check out the `prettier` documentation for more info on sharing configurations](https://prettier.io/docs/en/configuration.html#sharing-configurations).
