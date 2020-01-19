# node.js-typescript-boilerplate

## Quick boilerplate to start a node.js project with TypeScript, Prettier and ESLint (with Airbnb guide integrated) and absolute paths fully working.

---

## Instructions

- Clone the repository or run (node.js v8+)

```
npx degit hSel3triK/node.js-typescript-boilerplate project-name
```

- Enter the project folder

- Run

```
npm i
npm run start:update
npm run start:dev
```

You should see '1' appear in the console, meaning everything worked!

- Remove boilerplate code

The code inside src/ is just for testing purposes. Since you already verified it is working, modify it as you wish.

> You might also want to populate package.json with custom values, or perhaps remove or change any integration.

---

## Scripts usage

`start:dev`

This script is probably the one that is going to be used the most, and, by running it, it will run the TypeScript code inside src/ directly, with `ts-node-dev`.

`start:update`

This script does not actually run the code, it will update every single package of package.json, and will reinstall them, with the most updated versions of them. Should be run periodically.

`start:build`

This script transpiles the whole TypeScript code inside of src/ to another folder, called build/, which will contain the vanilla JavaScript counterpart of the code you wrote. It will clean the folder build/ before if you have one, so, this folder will always have only the latest code you wrote. After transpiling, it will call `node` with some arguments and will attempt to run the plain JavaScript transpiled code, being this the most effective script for production.

**You should not need to use any other scripts by default but these 3, the others are complementary, and make these ones actually work.**

---

## Integrations

Since this repository has inside of it included the libraries [ESLint](https://eslint.org/) and [Prettier](https://prettier.io/), I would recommend you to install the official extensions of these libraries for your desired text editor / IDE, in case they have one. It will make editing much more easier and in a way more integrated way.

I wil leave a link for these extensions in some popular text editors and IDEs

### ESLint

- [Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)

- [Atom](https://atom.io/packages/eslint)

- [WebStorm](https://www.jetbrains.com/help/webstorm/eslint.html)

### Prettier

- [Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

- [Atom](https://atom.io/packages/prettier-atom)

- [WebStorm](https://www.jetbrains.com/help/webstorm/prettier.html)
