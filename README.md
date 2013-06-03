# grunt-git-status

[![Build Status](https://travis-ci.org/nyfagel/grunt-git-status.png?branch=master)](https://travis-ci.org/nyfagel/grunt-git-status)

> Runs git status

Forked off [mikaelkaron/grunt-git-describe](https://github.com/mikaelkaron/grunt-git-describe).

## Getting Started
This plugin requires Grunt `~0.4.0`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-git-status --save-dev
```

One the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-git-status');
```

## The "git-status" task

### Overview
In your project's Gruntfile, add a section named `git-status` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  "git-status": {
    "options": {
      // Task-specific options go here.
    },
    "your_target": {
      // Target-specific file lists and/or options go here.
    },
  },
})
```

> Note that since this is a [multi-task](http://gruntjs.com/creating-tasks#multi-tasks) you have to have at least one target defined for `git-describe` (otherwise the task won't run)

### Options

#### options.prop
Type: `String`  
Default value: `''`

A string value that is used as a property name for storing the result of this task

#### options.cwd
Type: `String`  
Default value: `'.'`

A string value that is used to do set the current working directory when spawning the `git` command

#### options.failOnError
Type: `boolean`  
Default value: `true`

A boolean that allows Grunt to keep going if there's an error in this task. This is useful if your build isn't guaranteed to always be run from within a Git repo.

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
1.0.0 - First release, forked from grunt-git-describe, compatible with grunt `~0.4.0`
