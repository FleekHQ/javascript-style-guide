# Terminal's Javascript Style Guide

## Motivation

We should strive for an homogeneus codebase across our different apps and services, specially if we are planning to open-source part of it.

## Airbnb's Style Guide

Airbnb devs did a very detailed style guide for their javascript projects. [You can find it here](https://github.com/airbnb/javascript/tree/master/react). It is very standard nowadays and serves a a good starting point.

## How to install it into your projects

1. Run the following command to add the required packages:

`yarn add -D eslint eslint-config-airbnb-base eslint-plugin-import`

2. Then, create a file called `.eslintrc.js` in the root folder of your project and add the following code:

```
module.exports = {
    "extends": "airbnb-base"
};
```

3. Finally, install the eslint plugin for your text editor. [This is the package in the case of VS Code](https://github.com/Microsoft/vscode-eslint). Restart your editor after installing it. It should display red lines under any non-compliant code.

Note: This project has everything installed and you can just fork/clone it to use it as a base for other javascript projects.

## "But it's too much work to comply to all these standards >:("

Worry no more! You can make your editor auto-fix your offenses after each save.

### Instructions for VS Code

1. Go to user settings (or press `cmd/ctrl + ,`)

2. Click the `...` button and click `Open settings.json`.

3. Add the following line: `"eslint.autoFixOnSave": true`

4. Save the file and check if it works.
