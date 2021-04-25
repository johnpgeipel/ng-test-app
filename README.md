# NgTestApp

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 11.2.10.

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

## Deploy to Github Pages
[Tutorial Method #1](https://www.logic24by7.com/how-to-deploy-an-angular-app-to-github-pages/)

## Deploy Changes
`save changes > stage > commit > push to main`

`$ ng build --prod --base-href https://johnpgeipel.github.io/ng-test-app/`

`$ ngh --dir=dist/ng-test-app`
## Added ```deploy``` script to ```package.json```
This allows for the one step build and deployment to gh-pages with the command ```npm run deploy```. After making changes to `src`, add, commit and push to main branch, then run `npm run deploy` to update app.
```json
"scripts": {
    "ng": "ng",
    "start": "ng serve",
    "build": "ng build",
    "test": "ng test",
    "lint": "ng lint",
    "e2e": "ng e2e",
    "deploy": "ng build --prod --base-href https://johnpgeipel.github.io/ng-test-app/ && ngh --dir=dist/ng-test-app"
  },
```