<div align="center">
  <a href="http://fountainjs.io/">
    <img alt="FountainJS" src="http://fountainjs.io/assets/imgs/fountain.png" width="200">
  </a>
  <a href="https://docs.angularjs.org/guide">
    <img alt="AngularJS" src="http://fountainjs.io/assets/imgs/angular1.png" width="200">
  </a>
</div>

# SeedularJS - A Seed for AngularJS App Projects
> This seed allows you to easily start an AngularJS v1.6.x web app project.

> It's built off the Angular 1 sub-generator of the [Yeoman Fountain generator for webapps](https://github.com/FountainJS/generator-fountain-webapp).

> It uses [Gulp 4](http://gulpjs.com/) as a task manager.

> It compiles, minifies, concatenates, and injects all the needed files.

## The SeedularJS Layers
Below is the list of layers and their respective components you'll find inside SeedularJS:

### Web Tooling Layer
[![Gulp](http://fountainjs.io/assets/imgs/gulp.png)](https://github.com/FountainJS/generator-fountain-gulp)
[![ESLint](http://fountainjs.io/assets/imgs/eslint.png)](https://github.com/FountainJS/generator-fountain-eslint)
[![BrowserSync](http://fountainjs.io/assets/imgs/browsersync.png)](https://github.com/FountainJS/generator-fountain-browsersync)
[![Karma](http://fountainjs.io/assets/imgs/karma.png)](https://github.com/FountainJS/generator-fountain-karma)

### Module Management Layer
[![Bower](http://fountainjs.io/assets/imgs/bower.png)](https://github.com/FountainJS/generator-fountain-inject)

### JS Preprocessor Layer
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript">
  <img alt="JavaScript" src="https://upload.wikimedia.org/wikipedia/commons/9/99/Unofficial_JavaScript_logo_2.svg" width="200">
</a>

### CSS Preprocessor Layer
<a href="http://sass-lang.com">
  <img alt="Sass" src="http://sass-lang.com/assets/img/logos/logo-b6e1ef6e.svg" width="200">
</a>

### CSS Framework Layer
<a href="http://foundation.zurb.com/sites.html">
  <img alt="Foundation for Sites" src="http://foundation.zurb.com/assets/img/learn/features/svgs/code-reduction-01.svg" width="200">
</a>
<a href="http://fontawesome.io">
  <img alt="Font Awesome" src="https://pbs.twimg.com/profile_images/811760530956423168/UVaJOvEw_400x400.jpg" width="200">
</a>

## Getting Started
To get started you can simply clone the `seedularjs` repository and install its dependencies:

### Requirements
SeedularJS is to be used with Git, Node >= 7.10.0, NPM => 4.6.1, and Gulp CLI >= 1.3.0. You can check your version numbers with the following command:
```
git --version && node --version && npm --version && gulp --version
```

### Clone `seedularjs`
Clone the `seedularjs` repository using git:

```
git clone https://github.com/AmmoCan/seedularjs.git
cd seedularjs
```

If you just want to start a new project without the `seedularjs` commit history then you can do:

```
git clone --depth=1 https://github.com/AmmoCan/seedularjs.git <your-project-name>
```

The `depth=1` tells git to only pull down one commit worth of historical data.

### Install Dependencies
SeedularJS has two kinds of dependencies: Development Tools and AngularJS framework code. The tools help with the management and testing of the application.

* The tools are installed via `npm`, the [Node Package Manager](https://www.npmjs.com).
* The AngularJS and other framework code are installed via `bower`, a [client-side code package manager](https://bower.io).

Before you install anything make sure you are in the project's directory:
```
cd <your-project-name>
```

##### Install Tools:
```
npm install
```

##### Install Framework Code:
```
bower install
```
After both installs, there should now be two new folders in the project directory.

* `node_modules` - contains the npm packages for the tools needed
* `bower_components` - contains the AngularJS and other framework files needed

### Run the App
SeedularJS is preconfigured with a simple development web server via [Browser Sync](https://www.browsersync.io). The simplest way to start this server is:

#### Use NPM Scripts
- `npm run build` to build an optimized version of your application in /dist
- `npm run serve` to launch a Browser Sync server on your source files
- `npm run serve:dist` to launch a server on your optimized application
- `npm run test` to launch your unit tests with Karma
- `npm run test:auto` to launch your unit tests with Karma in watch mode

#### Or Gulp Tasks
- `gulp` or `gulp build`
- `gulp serve`
- `gulp serve:dist`
- `gulp test`
- `gulp test:auto`

**If you don't have [`gulp-cli`](https://www.npmjs.com/package/gulp-cli) installed in global, you should have this error:**
> /usr/local/lib/node_modules/gulp/bin/gulp.js:121
    gulpInst.start.apply(gulpInst, toRun);
TypeError: Cannot read property 'apply' of undefined
