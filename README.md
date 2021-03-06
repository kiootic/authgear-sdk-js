# Skygear SDK for JavaScript

[![@skygear/web](https://img.shields.io/npm/v/@skygear/web.svg?label=@skygear/web)](https://www.npmjs.com/package/@skygear/web)
[![@skygear/web](https://img.shields.io/npm/dt/@skygear/web.svg?label=@skygear/web)](https://www.npmjs.com/package/@skygear/web)
[![@skygear/react-native](https://img.shields.io/npm/v/@skygear/react-native.svg?label=@skygear/react-native)](https://www.npmjs.com/package/@skygear/react-native)
[![@skygear/react-native](https://img.shields.io/npm/dt/@skygear/react-native.svg?label=@skygear/react-native)](https://www.npmjs.com/package/@skygear/react-native)
[![Build Status](https://travis-ci.org/SkygearIO/skygear-SDK-JS.svg?branch=next)](https://travis-ci.org/SkygearIO/skygear-SDK-JS)
![License](https://img.shields.io/badge/license-Apache%202-blue)

## Documentation

View the API Reference at [https://skygeario.github.io/skygear-SDK-JS/](https://skygeario.github.io/skygear-SDK-JS/).

## Usage

### Web

```sh
$ npm install --save @skygear/web
```

### React Native

```sh
$ npm install --save @skygear/react-native
```

## Contributing

First, fork the repository.

```sh
$ git clone --branch next git@github.com:<myusername>/skygear-SDK-JS.git
$ cd skygear-SDK-JS
$ npm install
$ npm run lerna bootstrap
```

## Releasing

First, ensure `github-release` and `yarn` tool is installed.
Also, Git should be configured to be able to sign using GPG keys,
and npm should be logged in as appropriate user.

```sh
$ npm run prepare-new-release
# Edit the file new-release.
# It will be prepended to CHANGELOG.md
# So make sure the style is consistent.
$ vim new-release
$ GIT_USER=<github-username> GITHUB_TOKEN=<github-token> GIT_BRANCH=master SKYGEAR_VERSION=<new-version> ./scripts/release.sh
```
