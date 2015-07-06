# grunt-psi

> Automate running Google PageSpeed Insights and record metrics with Grunt

## Getting Started
This plugin requires Grunt `~0.4.5`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-psi --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-psi');
```

## The "psi" task

### Overview
In your project's Gruntfile, add a section named `psi` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  psi: {
    options: {
      // Task-specific options go here.
    }
  },
});
```

### Options

#### options.url
Type: `String`
Default value: `'http://localhost'`

Optional. Determines where the report will be stored. Currently, all PSI tests are run against localhost.

#### options.port
Type: `Integer`
Default value: `null`

Optional. The port required to reach localhost. Used by ngrok.

#### options.limit
Type: `Integer`
Default value: `10`

Optional. The limit of the number of rows of the report to display to console.

#### options.strategy
Type: `String`
Default value: `'desktop'`

Optional. Strategy to use when analyzing the page.

#### options.threshold
Type: `Integer`
Default value: `1`

Optional. Threshold score to pass the PageSpeed test.

### Usage Examples
```js
grunt.initConfig({
  psi: {
    options: {
        port: '4000'
    }
  }
});
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
_(Nothing yet)_
