# Monorepo using Yarn workspaces

## About this project -
A simple Signin / Signout with google that enables user to login with persisting state on page reload. Configured routing using Outlets.

This project uses three different monorepos: 
- `components` inside the `packages/components` for creating the components using tailwind css.
- `api` inside the `packages/api` configure the api calls such as firebase configuration that is responsible for exposing the methods for react-app to use.
- `app` folder in the root folder configures the react-app using `vite`. All the `components` and `api` folder contents can be linked to `app`.

## Project requirements and How to run the project?

- Yarn is required as this project uses a Yarn Workspaces, Install using `npm i -g yarn` command or download using https://classic.yarnpkg.com/lang/en/docs/install/#windows-stable

- Node version 16+ is required, `16.15.0` is used while initializing the application

- Install packages using `yarn install` in the root directory

- To build the components and start the app use `yarn start` in root directory.

- To build the components and build the react app for production use `yarn build`.

- To Preview the live version of the app how it will look and perform as deployed live in our local system use `yarn preview` in the root directory.

- For manually building the components only use `yarn build-components` in root directory.

- To run the react-app skipping the component build use yarn `start-app` in the root directory.

- This project uses
  - [Npm Run All](https://www.npmjs.com/package/npm-run-all) for executing the commands seqentially.
  - [Cross Env](https://www.npmjs.com/package/cross-env) for using enviroment variables across different platforms.

- Open the url http://localhost:3000 or  http://127.0.0.1:3000 in the browser to see the project.

- Live uploaded demo - https://648bf0660627fa2d7e2a0b77--frolicking-gumption-e2a171.netlify.app
