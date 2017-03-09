# John's Frontend - Documentation

This project is very much an early **Work in Progress**. So is this documentation.

John's Frontend is an Angular 2 template, intended as a starting point for web user interfaces commonly used in analytics and data projects (machine learning, search, NLP...).
  

## Project Goals

- Develop a standard, easy customizable template for search / machine learning project demos
    - Simple data entry forms
    - Search bar, search facets, and search results components
    - Dashboards with charts and graphs
- Learn the latest front-end technology


## Template Customization 

- Fork the project on GitHub or download a copy. Erase the .git folder to get rid of the template development history. 
Reinitialize git:

```bash
cd myproject
git init
# edit the .ts files as needed
git add .
git commit -m "Initial commit"
```

- Install the npm packages described in the ``package.json`` dependency file and verify that it works:

```shell
npm install
```

- Install Angular CLI:

```bash
npm install -g @angular/cli
ng help 
```

There is no need for ``ng new myproject``. I already used the [Angular CLI](https://cli.angular.io/) to create / customize the [folder structure / project layout](https://angular.io/docs/ts/latest/guide/style-guide.html#!#file-tree). This template was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.0.0-beta.32.3.


### Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. 


### Development server

Use `ng serve` to test your app on a development server. 

```bash
cd myproject
ng serve   
```

Navigate to [http://localhost:4200/](http://localhost:4200/). 
The app will automatically reload if you change any of the source files.

Shut it down manually with `Ctrl-C`.


### Code Scaffolding

Run ``ng generate component component-name`` to generate a new component. You can also use ``ng generate directive/pipe/service/class/module``.


### Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).


### Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
Before running the tests, make sure you are serving the app via `ng serve`.


### Production

Use the `ng build -prod` flag for a production build.


### Further Help and Alternative to Angular CLI

To get more help on the Angular CLI, use `ng help` or check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

If you do not want to use the Angular CLI, modify ``package.json`` as follows:

```json
"description": "...",
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
```

The Angular 2 quickstart captured many of the most useful commands in npm scripts:

* `npm start` - runs the compiler and a server at the same time, both in "watch mode".
* `npm run build` - runs the TypeScript compiler once.
* `npm run build:w` - runs the TypeScript compiler in watch mode; the process keeps running, awaiting changes to TypeScript files and re-compiling when it sees them.
* `npm run serve` - runs the [lite-server](https://www.npmjs.com/package/lite-server), a light-weight, static file server, written and maintained by [John Papa](https://github.com/johnpapa) and [Christopher Martin](https://github.com/cgmartin) with excellent support for Angular apps that use routing.

Here are the test related scripts:

* `npm test` - compiles, runs and watches the karma unit tests
* `npm run e2e` - compiles and run protractor e2e tests, written in Typescript (*e2e-spec.ts)


## Useful Links

### HTML Boilerplate

- The basic boilerplate was obtained from [Initializr](http://www.initializr.com/)'s version with [Bootstrap](http://getbootstrap.com/).
- I made some additions from [HTML5 Boilerplate](https://html5boilerplate.com/)


### [TypeScript](http://www.typescriptlang.org/)

Angular 2 uses TypeScript. Here is a basic example:

```typescript
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
```


### Angular 2

- [Angular](https://angular.io/)
- [Learning Angular](https://angular.io/docs/ts/latest/guide/learning-angular.html)
- [LearnAngular2.com](http://learnangular2.com)
- [Angular2.com](http://www.angular2.com/)
- [Angular 2 TutorialsPoint](https://www.tutorialspoint.com/angular2/index.htm)


### Rich UI components for Angular 2

- [Review of Angular UI components](https://www.infoq.com/articles/Angular2-TypeScript-High-Level-Overview)
- [PrimeNG](http://www.primefaces.org/primeng/#/)
- [Angular Material](https://material.angular.io/)
- [NG-Lightning](http://ng-lightning.github.io/ng-lightning/#/)


### Angular 2 with ASP.NET Core and Visual Studio

- [ASP.NET Core Angular 2 – Starter Kit – Visual Studio 2017 Project](http://myview.rahulnivi.net/asp-net-core-angular-2-starter-kit-visual-studio-2017-project/)
- [Movie-Review-Starter-Kit](https://github.com/rahulsahay19/MovieReviewStarterKit)
- [Build Angular 2 apps with TypeScript and Visual Studio Code](https://channel9.msdn.com/Events/Ignite/2016/BRK2193)
- [ASP.NET Core + Angular 2 template for Visual Studio](http://blog.stevensanderson.com/2016/10/04/angular2-template-for-visual-studio/)
- [Visual Studio 2015 Quickstart](https://angular.io/docs/ts/latest/cookbook/visual-studio-2015.html)
- [Editing TypeScript in Visual Studio Code](https://code.visualstudio.com/Docs/languages/typescript)
