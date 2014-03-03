Heroku Buildpack for Node.js, gulp.js, and bower
========================================

Usage
-----

- Set your Heroku app's buildpack URL to `https://github.com/davidmfoley/heroku-buildpack-nodejs-gulp-bower.git`. To be safe, you should really fork this and use your fork's URL.
- Run `heroku labs:enable user-env-compile` to enable environment variable support
- Run `heroku config:set NODE_ENV=production` to set your environment to `production` (or any other name)
- Add a Gulp task called `heroku:production` that builds your app

- Add a single line `Procfile` to the root to serve the app via node:

```
web: node index.js
```

(edit to fit your case)

Credits
-------

Inspired by [Deploying a Yeoman/Angular app to Heroku](http://www.sitepoint.com/deploying-yeomanangular-app-heroku/).

Forked from [heroku-buildpack-nodejs-gulp](https://github.com/timdp/heroku-buildpack-nodejs-gulp).

Which was forked from [heroku-buildpack-nodejs](https://github.com/heroku/heroku-buildpack-nodejs).

Heavily based on [heroku-buildpack-nodejs-grunt](https://github.com/mbuchetics/heroku-buildpack-nodejs-grunt).
