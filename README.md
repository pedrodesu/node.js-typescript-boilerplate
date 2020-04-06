# node.js-typescript-boilerplate

## Quick boilerplate to start a node.js project with TypeScript, Prettier and ESLint (with Airbnb guide integrated) and absolute paths fully working.

---

## Initial setup

- Clone the repository or run

```
git clone https://github.com/hSel3triK/node.js-typescript-boilerplate.git project-name # node.js v8+
```

- Enter the project folder

- Run

```
npm i # Install initial packages
npm run update # Update packages using pre-installed packages (npm-check-updates)
npm run start:dev # Run the project in development mode
```

You should see 'It is working.' appear in the console, meaning everything worked!

- Remove boilerplate code

The code inside src/ is just for testing purposes. Since you already verified it is working, modify it as you wish.
You can use `npm run clean` to wipe out the src folder, for a fresh project.
You might also want to populate package.json with custom values, or perhaps remove or change any integration.

> Keep in mind that for the project to work, you need a main file inside the src folder, called index.ts (changeable in package.json)

---

## Scripts usage

`start:dev`

This script is probably the one that is going to be used the most. It will run the TypeScript code inside src/ directly, with `ts-node-dev`. This script reloads as you modify and save your code and does not run JavaScript code directly, so it is good to be used for development and testing matters, in your localhost.

`start:production`

This script will call `node` with some arguments and will attempt to run the plain JavaScript transpiled code, being this the most effective script for production matters.

`update`

This script will update every single package of package.json, and will reinstall them, with the most updated versions of them. Should be run periodically.

`build`

This script transpiles the whole TypeScript code inside of src/ to another folder, called build/, which will contain the vanilla JavaScript counterpart of the code you wrote.

`clean`

This script will not be run quite often. It will delete everything inside the src/ folder, being the best way to start with a new, fresh project, removing the old code. Could be run to remove the template code that comes with the boilerplate.

---

## Integrations

Since this repository includes libraries and integrations ([ESLint](https://eslint.org/) and [Prettier](https://prettier.io/)), I would recommend you to install the official extensions of these libraries for your desired text editor / IDE, if they have one. It will make editing much easier and in a much more integrated way.

Links for these extensions in some popular text editors and IDEs:

### ESLint

- [Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)

- [Atom](https://atom.io/packages/eslint)

- [WebStorm](https://www.jetbrains.com/help/webstorm/eslint.html)

### Prettier

- [Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

- [Atom](https://atom.io/packages/prettier-atom)

- [WebStorm](https://www.jetbrains.com/help/webstorm/prettier.html)
