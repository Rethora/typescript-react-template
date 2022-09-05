# Front End Print

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

### Prerequisites

- Install nvm
- Install yarn

### Installation

- clone project
- `$ nvm install` => To use configured node version
- `$ yarn` => To install dependencies
- `$ yarn start` => To start development server on port 3000

### Conventional Commits

- This project uses [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)
- ex: `$ git commit -a -m"<type>[optional scope]: <description>"`
- `feat`: introduces a new feature to the codebase (this correlates with a MINORin SemVer es: 2.0.0 -> 2.1.0).
- `fix`: a bugfix in your codebase (this correlates with a PATCH in semVer es: 2.0.0 -> 2.0.1).
- `BREAKING CHANGE`: is a total change of your code, this is also can be used with a previous tag like BREAKING CHANGE: feat: <description> (this correlates with a MAJOR in SemVer es: 2.0.0 -> 3.0.0).
- `docs`: a change in the README or documentation
  refactor: a change in production code focused on upgrade code readability and style
- Try out the conventional commits vscode extension

### Changelog

- [standard-version](https://www.npmjs.com/package/standard-version)

- `$ yarn release --release-as <patch|minor|major>`
  - Updates CHANGELOG.md from conventional commits
  - Increments version number in package.json

### Notes

- When using nvm, you need to set the correct PATH before running the hooks
- Create a ~/.huskyrc
- Add the following to the file

```sh
# ~/.huskyrc
# This loads nvm.sh and sets the correct PATH before running hook
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
```
