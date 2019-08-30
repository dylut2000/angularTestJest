# AngularTestJest

Easy setup an [Angular](https://angular.io/) app with [Jest](https://jestjs.io/docs/en/getting-started) Testing Framework 

[Angular CLI](https://github.com/angular/angular-cli) version 8.3.0


# Steps

We are going to use [Jest](https://jestjs.io/docs/en/getting-started) and [jest-preset-angular](https://www.npmjs.com/package/jest-preset-angular) for this..

* Step 1 : Remove Karma related stuff (almost everything that has to do with Karma from the package json and the app)

```
npm remove karma karma-chrome-launcher karma-coverage-istanbul-reporter karma-jasmine karma-jasmine-html-reporter
```

```
rm ./karma.conf.js ./src/test.ts
```
<hr>

* Step 2 : Install [Jest](https://jestjs.io/docs/en/getting-started) and [jest-preset-angular](https://www.npmjs.com/package/jest-preset-angular)

```
npm i -D jest @types/jest @angular-builders/jest
```
<hr>

* step 3 : Update your Typescript configurations

In **tsconfig.spec.json** (src directory or project roots, used by Jest)<br>
1 . Replace **jasmine** in types array with **jest**<br>
2 . Remove **test.ts** from files array<br>
3 . Add **jest** to types array
<hr>

