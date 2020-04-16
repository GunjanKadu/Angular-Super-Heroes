<p align="center">
  <h3 align="center">Angular Super Heroes</h3>
  <p align="center">
    Example app with Angular 8 + Angular CLI + Angular Universal + i18n + Firebase
    <br>
    <br>
    :heart::heart::tada::tada::tada::tada::heart::heart:
    <br>
    <br>
    Base project made with much :heart:. Contains CRUD, patterns, generated library, and much more!
    <br>
    <br>
  </p>
</p>

## Demo

![](gif/Demo1.gif)

## What's included

- [x] CRUD: create, update and remove heroes with Firebase
- [x] Angular Universal (SSR)
- [x] Use of [preboot](https://github.com/angular/preboot) module to share state between browser and server
- [x] Security Headers using [helmet](https://helmetjs.github.io). Report [here](https://securityheaders.com/?q=https%3A%2F%2Fwww.angularexampleapp.com).
- [x] Internationalization with the official i18n. Separated builds for english and spanish.
- [x] Lazy loading modules
- [x] Service Workers enabled!
- [x] Example of Angular Resolver for Hero Detail
- [x] More logical directory structure (from [here](https://itnext.io/choosing-a-highly-scalable-folder-structure-in-angular-d987de65ec7))
- [x] Basic example library
- [x] Following the [best practices](https://angular.io/guide/styleguide)!
- [x] Search bar, to look for heroes
- [x] Custom loading page
- [x] Lazy loading images with [ng-lazyload-image](https://github.com/tjoskar/ng-lazyload-image)
- [x] Modal and toasts (snakbar)!
- [x] Scroll restoration and anchor examples
- [x] Responsive layout (flex layout module)
- [x] SASS (most common used functions and mixins) and BEM styles
- [x] Animations with [ng-animate](https://jiayihu.github.io/ng-animate/)
- [x] Angular Pipes
- [x] Interceptors and Events (Progress bar active, if a request is pending)
- [x] Modernizr (browser features detection)
- [x] Browser filter (Bowser) because of IE ^^
- [x] [Sentry](https://sentry.io)! (logs every error in the app)
- [x] Google Tag Manager
- [x] ES6 Promises and Observables
- [x] Unit tests with Jasmine and Karma including code coverage. Use of [ng-bullet](https://www.npmjs.com/package/ng-bullet), [karma-mocha-reporter](https://github.com/litixsoft/karma-mocha-reporter) and [ng-mocks](https://github.com/ike18t/ng-mocks)
- [x] End-to-end tests with Protractor

### Firebase

This repo is using Firebase. We use Cloud Firestore and Cloud Storage to handle CRUD operations over the heroes and to store their images. Also Hosting and Functions to deploy the app with Universal.

## Travis CI

We use Travis CI to run this tasks in order:

- Linter
- Unit tests
- End to end tests
- Build for production of browser and server
- Validate that server generated using curl
- Sonar
- Deploy to Firebase

## Quick start

**WARNING**

> Verify that you are running node 10.16.0 by running node -v in a terminal/console window. Older versions produce errors, but newer versions are fine.

```bash
npm i
npm start
```

| Tasks                      | Description                                                                                          |
| -------------------------- | ---------------------------------------------------------------------------------------------------- |
| npm start                  | Start the app in development mode with the english language only                                     |
| npm start:es               | Start the app in development mode with the spanish language only                                     |
| start:ssr                  | Start the server like SSR                                                                            |
| extract-i18n               | Extract all messages from templates and ts files and update the language files with new translations |
| npm run lint               | Run the linter (tslint)                                                                              |
| npm run test               | Run all unit tests with karma and jasmine                                                            |
| npm run test:app:watch     | Run app unit tests and wait for changes                                                              |
| npm run test:library:watch | Run library unit tests and wait for changes                                                          |
| npm run e2e                | Run end to end tests with protractor                                                                 |
| npm run build:prod:en      | Build the app for production with english translations                                               |
| npm run build:prod:es      | Build the app for production with spanish translations                                               |
| npm run build:server:prod  | Build the server version for production                                                              |
| npm run compile:server     | Compiles the server with webpack                                                                     |
| npm run build:ssr          | Complete task with all the build subtasks for SSR                                                    |
| npm run build:library      | Build the library                                                                                    |
| npm run serve:ssr          | Start the node server for angular universal                                                          |
| npm run validate:server    | Script that validate if server generated previously starts without error                             |
| npm run bundle-report      | Build and run webpack-bundle-analyzer over stats json                                                |
| npm run release:minor      | Create a new minor release using standard-version                                                    |
| npm run release:major      | Create a new major release using standard-version                                                    |
| npm run ci                 | Execute linter, tests and production builds                                                          |
| npm run deploy             | Build the app and deploy it to firebase hosting                                                      |

## Creators

**Gunjan Kadu**

- <https://github.com/GunjanKadu>
