# React Create App Quickstart
> Minimal React app template that uses CI to deploy to Github Pages

[![GH Pages Deploy](https://github.com/MichaelCurrin/react-create-app-quickstart/workflows/GH%20Pages%20Deploy/badge.svg)](https://github.com/MichaelCurrin/react-create-app-quickstart/actions)
[![GitHub tag](https://img.shields.io/github/tag/MichaelCurrin/react-create-app-quickstart)](https://github.com/MichaelCurrin/react-create-app-quickstart/tags/)
[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](#license)

[![Use this template](https://img.shields.io/badge/Use_this_template-2ea44f?style=for-the-badge)](https://github.com/MichaelCurrin/react-create-app-quickstart/generate)

[![View demo - React Create App Quickstart](https://img.shields.io/badge/View_demo-React%20Create%20App%20Quickstart-green?style=for-the-badge)](https://michaelcurrin.github.io/react-create-app-quickstart/)


## About

- A simple React scaffold, including setup and run instructions.
- Use as a reference for new or existing applications.
- Add a copy to your repos with _Use this template_ button.
- This project is based on the files generated by React CLI's [create-react-app](#create-a-fresh-project) command.


## Documentation

Follow the setup instructions using this repo a template copied to your own repos.

Then you can run a start command to build and run the app, then you can view the app in the browser.

See [docs](/docs/README.md).


## How a React project works

- A React app typically runs as a _Node.js_ server, especially locally. This uses a compile step and runs from memory - there is no `build` directory used.
- The app can be compiled to a _build_ directory for running as a static site - this means you can deploy to GitHub Pages or Netlify.
- React uses `.js` or `.jsx` files with _JSX_ syntax (HTML inside JavaScript). These cannot be run directly. But these are transpiled (or compiled) to plain JavaScript by the `react-script build` command. Babel is used for that transpiling, but it is not necessary to use specify it directory as it is covered through the direct dependencies.


## Resources

- [React](https://reactjs.org/) homepage
- [react](https://www.npmjs.com/package/react) package on NPM
- [create-react-app.dev](https://create-react-app.dev/) homepage
    - [Getting started](https://create-react-app.dev/docs/getting-started/)
- [facebook/create-react-app](https://github.com/facebook/create-react-app) repo


## Create a fresh project

This project used skeleton setup generated below as a starting point.

Install [Node.js](https://gist.github.com/MichaelCurrin/aa1fc56419a355972b96bce23f3bccba).

Run the `npx` command to install and run `create-react-app`.

```sh
$ npx create-react-app my-app
$ cd my-app
```

You'll get a project setup like this:

```
my-app
├── README.md
├── node_modules
├── package.json
├── .gitignore
├── public
│   ├── favicon.ico
│   ├── index.html
│   └── manifest.json
└── src
    ├── App.css
    ├── App.js
    ├── App.test.js
    ├── index.css
    ├── index.js
    ├── logo.svg
    └── serviceWorker.js
    └── setupTests.js
```

Start the application.

```
$ npm start
```


## Development

Notes about this project.

- It is better to set state through a method rather than by changing state directly.
- The Foo component is based on part of this video: [Get started with React in under 10 minutes](https://youtu.be/K02AkMbV1HM)
- This project uses 3 main dependencies, which were included with the quickstart
    - `react` - for the core application.
    - `react-dom` - for using `ReactDom` in [App.js](/src/App.js).
    - `react-scripts` - used to setup the `script` commands in [package.json](/package.json).
- There are 3 testing libraries - these were moved to dev dependencies.
- When running the `build` command, the `NODE_ENV` value will be set to `production` by React - see [React docs - Adding custom env variables](https://create-react-app.dev/docs/adding-custom-environment-variables/).
- Homepage
    - The `homepage` value is set [package.json](/package.json) and used on the build - see `index.html` in the output includes `src="/react-create-app-quickstart/static/js/..."` for example.
    - This is necessary for GH Pages build to work correctly on a subpath.
    - It doesn't seem to matter whether the value is just `/react-create-app-quickstart/` or the full `https://michaelcurrin.github.io/react-create-app-quickstart/`.
    - Customize this value for other repos.


## License

Released under [MIT](/LICENSE).
