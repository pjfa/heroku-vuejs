# Heroku Vue.js sample

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

---

## TL;DR

```bash
# Create your application using `vue-cli` with `pwa` template
vue init pwa YOUR-HEROKU-DYNO-NAME

# Navigate to your application folder and create a Git repository
cd YOUR-HEROKU-DYNO-NAME/
git init

# Create a Heroku Dyno using Node.js buildpack
heroku apps:create YOUR-HEROKU-DYNO-NAME --buildpack https://github.com/heroku/heroku-buildpack-nodejs

# Add static buildpack as secondary
heroku buildpacks:add https://github.com/heroku/heroku-buildpack-static --index 2

# Create `static.json` with Heroku buildpack settings
# https://github.com/magnobiet/heroku-vuejs/blob/master/static.json

# Add `postinstall` script with build command to your `package.json`
# https://github.com/magnobiet/heroku-vuejs/blob/master/package.json#L15

# Commit all changes
git add .
git commit -m "Initial commit"

# Deploy your application
git push heroku master

# In your browser navigate to https://YOUR-HEROKU-DYNO-NAME.herokuapp.com/
```

### References

- https://github.com/vuejs/vue-cli
- https://github.com/vuejs-templates/pwa
- https://github.com/heroku/heroku-buildpack-nodejs
- https://github.com/heroku/heroku-buildpack-static
