# Template-Node-TS-Jest

This is a template project for a faster start on a NodeJS Typescript project using Jest to test.
Code samples, vscode launch configs, example tests etc are included.

# Steps to use

1. Clone/fork repo
2. `npm install`
3. `package.json` - replace all `TODO` with relevant info
4. `__tests__/` - add your tests
5. `index.ts` - add your code
6. delete irrelevant examples (`src/core/`, `src/utils/`, `config/`)
7. Run/Test: `npm start` / `npm test`! (Or with vscode launch configs)

# Fork Changes from original [Jon]

Original repo - see it for steps used to create this project template.
https://github.com/mtiller/ts-jest-sample

Changes:

- `launch.json`
  - Didn't work on windows, seems like assums mac/linux?
  - Used this launch.json instead: \([master][new-launch-json-master] | [actual commit taken][new-launch-json-commit]\)
  - Added ts-node launch configs (debugger)
- `tsconfig.json`
  - Changed target to `es2017` + include `"lib": ["es2017"]`
  - Removed `strict` + `noImplicitAny` restrictions
  - Added `ts-node` section (`transpileOnly` - doesn't type check)
- Package.json
  - added `ts-node`
- `.gitignore`
  - Used [Github node GitIgnore](https://github.com/github/gitignore/blob/master/Node.gitignore)
  - Removed `.npmignore` (`.gitignore` will be used and is much more complete)
- `Readme`
  - Added this section
- Source code
  - Various minor changes to example code
-
- Updated packages to latest [17/Feb/23]

<!-- Markdown Links -->

[new-launch-json-master]: https://github.com/Lemoncode/jest-vs-code-debugging-example/blob/master/custom-solution-jest-config-file/01-implemented/.vscode/launch.json
[new-launch-json-commit]: https://github.com/Lemoncode/jest-vs-code-debugging-example/blob/1f6a82eb773bc96e8f75709cb41d4da8cc8858ec/custom-solution-jest-config-file/01-implemented/.vscode/launch.json
