# Angular

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 20.0.0-next.5 as follows:

```
alexeagle@aspect-build repros % npx @angular/cli@20.0.0-next.5 new angular --create-application=false --skip-install
CREATE angular/README.md (1477 bytes)
CREATE angular/.editorconfig (314 bytes)
CREATE angular/.gitignore (587 bytes)
CREATE angular/angular.json (139 bytes)
CREATE angular/package.json (956 bytes)
CREATE angular/tsconfig.json (888 bytes)
CREATE angular/.vscode/extensions.json (130 bytes)
CREATE angular/.vscode/launch.json (470 bytes)
CREATE angular/.vscode/tasks.json (938 bytes)
    Successfully initialized git.
alexeagle@aspect-build repros % cd angular
alexeagle@aspect-build angular % echo "hoist=false" > .npmrc
alexeagle@aspect-build angular % npx @angular/cli@20.0.0-next.5 generate library my-lib --skip-install
CREATE projects/my-lib/README.md (1447 bytes)
CREATE projects/my-lib/ng-package.json (155 bytes)
CREATE projects/my-lib/package.json (224 bytes)
CREATE projects/my-lib/tsconfig.lib.json (475 bytes)
CREATE projects/my-lib/tsconfig.lib.prod.json (401 bytes)
CREATE projects/my-lib/tsconfig.spec.json (434 bytes)
CREATE projects/my-lib/src/public-api.ts (70 bytes)
CREATE projects/my-lib/src/lib/my-lib.spec.ts (522 bytes)
CREATE projects/my-lib/src/lib/my-lib.ts (194 bytes)
UPDATE angular.json (974 bytes)
UPDATE package.json (1032 bytes)
UPDATE tsconfig.json (960 bytes)
alexeagle@aspect-build angular % npx pnpm@8 install
 WARN  3 deprecated subdependencies found: glob@7.2.3, inflight@1.0.6, rimraf@3.0.2
Packages: +513
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Progress: resolved 612, reused 513, downloaded 0, added 513, done
node_modules/.pnpm/@parcel+watcher@2.5.1/node_modules/@parcel/watcher: Running install script, done in 37ms
node_modules/.pnpm/esbuild@0.25.2/node_modules/esbuild: Running postinstall script, done in 329ms
node_modules/.pnpm/msgpackr-extract@3.0.3/node_modules/msgpackr-extract: Running install script, done in 508ms
node_modules/.pnpm/lmdb@3.2.6/node_modules/lmdb: Running install script, done in 557ms

dependencies:
+ @angular/common 20.0.0-next.6
+ @angular/compiler 20.0.0-next.6
+ @angular/core 20.0.0-next.6
+ @angular/forms 20.0.0-next.6
+ @angular/platform-browser 20.0.0-next.6
+ @angular/router 20.0.0-next.6
+ rxjs 7.8.2
+ tslib 2.8.1
+ zone.js 0.15.0

devDependencies:
+ @angular/build 20.0.0-next.5
+ @angular/cli 20.0.0-next.5
+ @angular/compiler-cli 20.0.0-next.6
+ @types/jasmine 5.1.7
+ jasmine-core 5.6.0
+ karma 6.4.4
+ karma-chrome-launcher 3.2.0
+ karma-coverage 2.2.1
+ karma-jasmine 5.1.0
+ karma-jasmine-html-reporter 2.1.0
+ ng-packagr 20.0.0-next.6
+ typescript 5.8.3

Done in 6.5s
alexeagle@aspect-build angular % ./node_modules/.bin/ng test my-lib
Initial chunk files     | Names                |  Raw size
chunk-UR5JXVJH.js       | -                    |   2.17 MB |
polyfills.js            | polyfills            |   1.01 MB |
test_main.js            | test_main            | 240.30 kB |
jasmine-cleanup-1.js    | jasmine-cleanup-1    |  65.98 kB |
spec-lib-my-lib.spec.js | spec-lib-my-lib.spec |   2.50 kB |
chunk-TTULUY32.js       | -                    |   1.99 kB |
jasmine-cleanup-0.js    | jasmine-cleanup-0    | 659 bytes |

                        | Initial total        |   3.49 MB

Application bundle generation complete. [1.157 seconds]

Watch mode enabled. Watching for file changes...
15 04 2025 14:30:19.913:WARN [karma]: No captured browser, open http://localhost:9876/
15 04 2025 14:30:20.108:INFO [karma-server]: Karma v6.4.4 server started at http://localhost:9876/
15 04 2025 14:30:20.108:INFO [launcher]: Launching browsers Chrome with concurrency unlimited
15 04 2025 14:30:20.111:INFO [launcher]: Starting browser Chrome
15 04 2025 14:30:21.580:INFO [Chrome 135.0.0.0 (Mac OS 10.15.7)]: Connected on socket hCGRJpWhU_aaurDzAAAB with id 37609754
Chrome 135.0.0.0 (Mac OS 10.15.7): Executed 1 of 1 SUCCESS (0.018 secs / 0.015 secs)
```

Then Bazel files are added in a subsequent commit.

## Development server

To start a local development server, run:

```bash
ng serve
```

Once the server is running, open your browser and navigate to `http://localhost:4200/`. The application will automatically reload whenever you modify any of the source files.

## Code scaffolding

Angular CLI includes powerful code scaffolding tools. To generate a new component, run:

```bash
ng generate component component-name
```

For a complete list of available schematics (such as `components`, `directives`, or `pipes`), run:

```bash
ng generate --help
```

## Building

To build the project run:

```bash
ng build
```

This will compile your project and store the build artifacts in the `dist/` directory. By default, the production build optimizes your application for performance and speed.

## Running unit tests

To execute unit tests with the [Karma](https://karma-runner.github.io) test runner, use the following command:

```bash
ng test
```

## Running end-to-end tests

For end-to-end (e2e) testing, run:

```bash
ng e2e
```

Angular CLI does not come with an end-to-end testing framework by default. You can choose one that suits your needs.

## Additional Resources

For more information on using the Angular CLI, including detailed command references, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.
