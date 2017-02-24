# Side Project Documentation

**Work in Progress**


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

https://angular.io/docs/ts/latest/guide/style-guide.html#!#file-tree



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





### Rich UI components for Angular 2:

[Review of UI components](https://www.infoq.com/articles/Angular2-TypeScript-High-Level-Overview)

[PrimeNG](http://www.primefaces.org/primeng/#/]

[Angular Material](https://material.angular.io/)

[NG-Lightning](http://ng-lightning.github.io/ng-lightning/#/)



### HTTPS Certifactes

https://letsencrypt.org/docs/client-options/ 