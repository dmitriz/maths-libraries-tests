# min-karma-webpack
Testing Mathematics libraries

[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)

# Tech stack

## Karma
[Karma](http://karma-runner.github.io/0.13/index.html) is a JavaScript Test Runner, one of the most popular and friendliest for beginners. The most notable advantage of Karma is *testing in real browsers*. [See my StackOverflow answer for more information about Karma usage.](http://stackoverflow.com/a/29619467/1614973)

## Webpack
[Webpack](https://webpack.github.io/) is a popular JavaScript/NodeJS Module Bundler.


# FAQ

## But I already run NodeJS! Why do I need Webpack to load my modules just to test them?
Karma runs your tests as separate JavaScript files in real browsers
that don't natively support modules.
So you need a bundler like Webpack (or Browserify) to pre-process your modules beforehand.
This is achieved by the [excellent preprocessor support from Karma](https://karma-runner.github.io/0.13/config/preprocessors.html)

## But what if I only need my modules to run with NodeJS?
You may want to re-use some of your modules later in web applications.
By running your tests in real browsers now you make them future-proof.

## Features
- **No webpack config file needed for testing!** (You still get one as bonus. ;-)
- Minimal functional Karma config file.
- Minimal testing demo examples.

## If you are new to Node
[Download and Install Node.js](https://nodejs.org/download/), see [How do I get started with Node.js](http://stackoverflow.com/questions/2353818/how-do-i-get-started-with-node-js) for more information.


## Setting up
### Clone
```sh
git clone https://github.com/dmitriz/maths-libraries-tests
```
or simply [Download this Repository](https://github.com/dmitriz/maths-libraries-tests/archive/master.zip),
unzip it and `cd maths-libraries-tests-master`.


### Install dependencies
```sh
npm install
```

## Getting started
Run your tests:
```sh
karma start
```
Now try to edit files inside `demo` folder and see how karma is watching and updating your test results.

Enjoy!
