# Side Project Documentation

This project is very much still a **Work in Progress**. So is this documentation.


## Step by Step

### Setup

```
git init
git add .
git commit -m "Initial commit"
```

### HTML Boilerplate

- download boilerplate from [Initializr](http://www.initializr.com/)
(get the version with [Bootstrap](http://getbootstrap.com/)).

- add extra files from https://html5boilerplate.com/


### [TypeScript](http://www.typescriptlang.org/)

// interface
interface Person {
    firstName: string;
    lastName: string;
}

function greeter(person: Person) {
    return "Hello, " + person.firstName + " " + person.lastName;
}

var user = { firstName: "Jane", lastName: "User" };

document.body.innerHTML = greeter(user);

class Student {
    fullName: string;
    constructor(public firstName, public middleInitial, public lastName) {
        this.fullName = firstName + " " + middleInitial + " " + lastName;
    }
}

interface Person {
    firstName: string;
    lastName: string;
}

function greeter(person : Person) {
    return "Hello, " + person.firstName + " " + person.lastName;
}

var user = new Student("Jane", "M.", "User");

document.body.innerHTML = greeter(user);



### Angular 2


https://angular.io/docs/ts/latest/guide/learning-angular.html


[Angular](https://angular.io/)

[Learnangular2.com](http://learnangular2.com)

[Angular2.com](http://www.angular2.com/)

http://myview.rahulnivi.net/asp-net-core-angular-2-starter-kit-visual-studio-2017-project/

https://github.com/rahulsahay19/MovieReviewStarterKit

https://channel9.msdn.com/Events/Ignite/2016/BRK2193

http://blog.stevensanderson.com/2016/10/04/angular2-template-for-visual-studio/

https://www.tutorialspoint.com/angular2/index.htm


### create folder structure

https://cli.angular.io/

https://angular.io/docs/ts/latest/guide/style-guide.html#!#file-tree


### Angular CLI

```bash
$ npm install -g @angular/cli

$ ng help

ng new PROJECT_NAME
cd PROJECT_NAME
ng serve

```


This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.0.0-beta.32.3.

## Development server
Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive/pipe/service/class/module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
Before running the tests make sure you are serving the app via `ng serve`.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).



### npm package.json` when not using Angular CLI

(from quickstart)

"description": "QuickStart package.json from the documentation, supplemented with testing support",
  "scripts": {
    "build": "tsc -p src/",
    "build:watch": "tsc -p src/ -w",
    "build:e2e": "tsc -p e2e/",
    "serve": "lite-server -c=bs-config.json",
    "serve:e2e": "lite-server -c=bs-config.e2e.json",
    "prestart": "npm run build",
    "start": "concurrently \"npm run build:watch\" \"npm run serve\"",
    "pree2e": "npm run build:e2e",
    "e2e": "concurrently \"npm run serve:e2e\" \"npm run protractor\" --kill-others --success first",
    "preprotractor": "webdriver-manager update",
    "protractor": "protractor protractor.config.js",
    "pretest": "npm run build",
    "test": "concurrently \"npm run build:watch\" \"karma start karma.conf.js\"",
    "pretest:once": "npm run build",
    "test:once": "karma start karma.conf.js --single-run",
    "lint": "tslint ./src/**/*.ts -t verbose"
  },



### Install npm packages

Install the npm packages described in the `package.json` and verify that it works:

```shell
npm install
npm start
```

>Doesn't work in _Bash for Windows_ which does not support servers as of January, 2017.

The `npm start` command first compiles the application, 
then simultaneously re-compiles and runs the `lite-server`.
Both the compiler and the server watch for file changes.

Shut it down manually with `Ctrl-C`.

### npm scripts

We've captured many of the most useful commands in npm scripts defined in the `package.json`:

* `npm start` - runs the compiler and a server at the same time, both in "watch mode".
* `npm run build` - runs the TypeScript compiler once.
* `npm run build:w` - runs the TypeScript compiler in watch mode; the process keeps running, awaiting changes to TypeScript files and re-compiling when it sees them.
* `npm run serve` - runs the [lite-server](https://www.npmjs.com/package/lite-server), a light-weight, static file server, written and maintained by
[John Papa](https://github.com/johnpapa) and
[Christopher Martin](https://github.com/cgmartin)
with excellent support for Angular apps that use routing.

Here are the test related scripts:
* `npm test` - compiles, runs and watches the karma unit tests
* `npm run e2e` - compiles and run protractor e2e tests, written in Typescript (*e2e-spec.ts)


## Visual Studio Code + TypeScript

https://code.visualstudio.com/Docs/languages/typescript#_hiding-derived-javascript-files


## Visual Studio integration

https://angular.io/docs/ts/latest/cookbook/visual-studio-2015.html

http://blog.stevensanderson.com/2016/10/04/angular2-template-for-visual-studio/

```bash
npm install -g typescript@2.0
```



### Rich UI components for Angular 2

[Review of UI components](https://www.infoq.com/articles/Angular2-TypeScript-High-Level-Overview)

[PrimeNG](http://www.primefaces.org/primeng/#/]

[Angular Material](https://material.angular.io/)

[NG-Lightning](http://ng-lightning.github.io/ng-lightning/#/)



### HTTPS Certificate Generation

https://letsencrypt.org/docs/client-options/ 