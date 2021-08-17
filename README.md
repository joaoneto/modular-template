## Modular template

This template is used to bootstrap a js stack monorepo packages.
The workspace configured is `packages`, and can be changed and incremented changing the prop workspaces in `package.json` and `lerna.json`.

### eslint

All code in package dir is validated with root `.eslint.json` rules, and it can be extended in each one package, justing placing a local `.eslint.json`.

### prettier
All code in package dir is formatted acording with recommended prettier format, with some additional behaviours in `.prettierrc`, respecting the eslint rules also.

### VSCode config

This project, once oppened in VSCode, is configured to automaticaly formats the code on save with the specified eslint rules.

### Lerna

Lerna can handle parallel executions in many packages into the workspace. If you don't want to do this, just remove the lerna package dependency in the `package.json`.
