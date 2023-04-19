# Introduction to npm

npm is a package manager for Node.js. It allows you to easily install and manage packages, which are libraries or modules that you can use in your Node.js projects. npm is also used to manage dependencies for your projects, making it easy to install and update packages that your project depends on.

# Installation

To use npm, you need to have Node.js installed on your machine. You can download Node.js from the official website at [https://nodejs.org/](https://nodejs.org/). Once you have Node.js installed, npm is automatically installed with it.

To verify that npm is installed, open a terminal or command prompt and type:

`npm --version`

This will prompt you to enter information about your project, such as the name, version, description, and author. You can press enter to accept the default values or enter your own values.

# Installing packages

Once you have a package.json file, you can use npm to install packages. To install a package from the npm registry, open a terminal or command prompt, navigate to the root directory of your project, and type:

`npm install <package-name>`

Replace `<package-name>` with the name of the package you want to install. For example, to install the *React* library, you would type:

`npm install react`

We can also abbreviate the command to:

`npm i react`