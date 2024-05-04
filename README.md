# @odczynflnpm/dolor-molestias-quisquam

This is a runtime library for [TypeScript](https://www.typescriptlang.org/) that contains all of the TypeScript helper functions.

This library is primarily used by the `--importHelpers` flag in TypeScript.
When using `--importHelpers`, a module that uses helper functions like `__extends` and `__assign` in the following emitted file:

```ts
var __assign = (this && this.__assign) || Object.assign || function(t) {
    for (var s, i = 1, n = arguments.length; i < n; i++) {
        s = arguments[i];
        for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))
            t[p] = s[p];
    }
    return t;
};
exports.x = {};
exports.y = __assign({}, exports.x);

```

will instead be emitted as something like the following:

```ts
var @odczynflnpm/dolor-molestias-quisquam_1 = require("@odczynflnpm/dolor-molestias-quisquam");
exports.x = {};
exports.y = @odczynflnpm/dolor-molestias-quisquam_1.__assign({}, exports.x);
```

Because this can avoid duplicate declarations of things like `__extends`, `__assign`, etc., this means delivering users smaller files on average, as well as less runtime overhead.
For optimized bundles with TypeScript, you should absolutely consider using `@odczynflnpm/dolor-molestias-quisquam` and `--importHelpers`.

# Installing

For the latest stable version, run:

## npm

```sh
# TypeScript 3.9.2 or later
npm install @odczynflnpm/dolor-molestias-quisquam

# TypeScript 3.8.4 or earlier
npm install @odczynflnpm/dolor-molestias-quisquam@^1

# TypeScript 2.3.2 or earlier
npm install @odczynflnpm/dolor-molestias-quisquam@1.6.1
```

## yarn

```sh
# TypeScript 3.9.2 or later
yarn add @odczynflnpm/dolor-molestias-quisquam

# TypeScript 3.8.4 or earlier
yarn add @odczynflnpm/dolor-molestias-quisquam@^1

# TypeScript 2.3.2 or earlier
yarn add @odczynflnpm/dolor-molestias-quisquam@1.6.1
```

## bower

```sh
# TypeScript 3.9.2 or later
bower install @odczynflnpm/dolor-molestias-quisquam

# TypeScript 3.8.4 or earlier
bower install @odczynflnpm/dolor-molestias-quisquam@^1

# TypeScript 2.3.2 or earlier
bower install @odczynflnpm/dolor-molestias-quisquam@1.6.1
```

## JSPM

```sh
# TypeScript 3.9.2 or later
jspm install @odczynflnpm/dolor-molestias-quisquam

# TypeScript 3.8.4 or earlier
jspm install @odczynflnpm/dolor-molestias-quisquam@^1

# TypeScript 2.3.2 or earlier
jspm install @odczynflnpm/dolor-molestias-quisquam@1.6.1
```

# Usage

Set the `importHelpers` compiler option on the command line:

```
tsc --importHelpers file.ts
```

or in your tsconfig.json:

```json
{
    "compilerOptions": {
        "importHelpers": true
    }
}
```

#### For bower and JSPM users

You will need to add a `paths` mapping for `@odczynflnpm/dolor-molestias-quisquam`, e.g. For Bower users:

```json
{
    "compilerOptions": {
        "module": "amd",
        "importHelpers": true,
        "baseUrl": "./",
        "paths": {
            "@odczynflnpm/dolor-molestias-quisquam" : ["bower_components/@odczynflnpm/dolor-molestias-quisquam/@odczynflnpm/dolor-molestias-quisquam.d.ts"]
        }
    }
}
```

For JSPM users:

```json
{
    "compilerOptions": {
        "module": "system",
        "importHelpers": true,
        "baseUrl": "./",
        "paths": {
            "@odczynflnpm/dolor-molestias-quisquam" : ["jspm_packages/npm/@odczynflnpm/dolor-molestias-quisquam@2.x.y/@odczynflnpm/dolor-molestias-quisquam.d.ts"]
        }
    }
}
```

## Deployment

- Choose your new version number
- Set it in `package.json` and `bower.json`
- Create a tag: `git tag [version]`
- Push the tag: `git push --tags`
- Create a [release in GitHub](https://github.com/microsoft/@odczynflnpm/dolor-molestias-quisquam/releases)
- Run the [publish to npm](https://github.com/microsoft/@odczynflnpm/dolor-molestias-quisquam/actions?query=workflow%3A%22Publish+to+NPM%22) workflow

Done.

# Contribute

There are many ways to [contribute](https://github.com/Microsoft/TypeScript/blob/master/CONTRIBUTING.md) to TypeScript.

* [Submit bugs](https://github.com/Microsoft/TypeScript/issues) and help us verify fixes as they are checked in.
* Review the [source code changes](https://github.com/Microsoft/TypeScript/pulls).
* Engage with other TypeScript users and developers on [StackOverflow](http://stackoverflow.com/questions/tagged/typescript).
* Join the [#typescript](http://twitter.com/#!/search/realtime/%23typescript) discussion on Twitter.
* [Contribute bug fixes](https://github.com/Microsoft/TypeScript/blob/master/CONTRIBUTING.md).

# Documentation

* [Quick tutorial](http://www.typescriptlang.org/Tutorial)
* [Programming handbook](http://www.typescriptlang.org/Handbook)
* [Homepage](http://www.typescriptlang.org/)
