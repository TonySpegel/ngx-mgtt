# NGX-MQTT Test Project

## Current behavior
While trying to install the dependency [ngx-mqtt](https://github.com/sclausen/ngx-mqtt) an error occurs.
This happens on a freshly created Angular project. The error is as follows:
```bash
npm install ngx-mqtt --save

npm ERR! code 1
npm ERR! path /Users/tony/Dev/work/e-paper/ngx-mqtt-test/node_modules/ngx-mqtt
npm ERR! command failed
npm ERR! command sh -c node postinstall
npm ERR! [Error: ENOENT: no such file or directory, open '../../node_modules/@angular-devkit/build-angular/src/angular-cli-files/models/webpack-configs/browser.js'] {
npm ERR!   errno: -2,
npm ERR!   code: 'ENOENT',
npm ERR!   syscall: 'open',
npm ERR!   path: '../../node_modules/@angular-devkit/build-angular/src/angular-cli-files/models/webpack-configs/browser.js'
npm ERR! }
npm ERR! /Users/tony/Dev/work/e-paper/ngx-mqtt-test/node_modules/ngx-mqtt/postinstall.js:33
npm ERR!     throw err;
npm ERR!     ^
npm ERR!
npm ERR! [Error: ENOENT: no such file or directory, open '../../node_modules/@angular-devkit/build-angular/src/angular-cli-files/models/webpack-configs/browser.js'] {
npm ERR!   errno: -2,
npm ERR!   code: 'ENOENT',
npm ERR!   syscall: 'open',
npm ERR!   path: '../../node_modules/@angular-devkit/build-angular/src/angular-cli-files/models/webpack-configs/browser.js'
npm ERR! }

npm ERR! A complete log of this run can be found in:
npm ERR!     /Users/tony/.npm/_logs/2021-03-08T08_04_07_732Z-debug.log
```
## Expected behavior
Being able to install and use the dependency with the latest Angular version (11.2.3 in this case)

## Minimal working example
[Link to this repo](https://github.com/TonySpegel/ngx-mgtt-test)

## What is the motivation / use case for changing the behavior?
Being able to use this dependency without having to change paths by yourself

## Environment
```
ngx-mgtt: 
none, it fails to install (so I'd say it is the latest which would be 6.13.3 as of today)
Angular: 11.2.3
Angular CLI: 11.2.2
Node: v15.10.0
NPM: 7.6.0
Broker: HiveMQ
```

## Steps to reproduce the problem

1. clone this repository `git clone https://github.com/TonySpegel/ngx-mgtt-test.git`
2. enter the cloned directory `cd ngx-mgtt-test`
3. Install the dependency `npm install ngx-mqtt --save`
4. See the error mentioned above


This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 11.2.2.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
