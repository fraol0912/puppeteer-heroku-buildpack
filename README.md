# puppeteer-heroku-buildpack

**This fork of the [CoffeeAndCode buildpack](https://github.com/CoffeeAndCode/puppeteer-heroku-buildpack) and adds support for Fira code font.**

Installs dependencies needed in order to run puppeteer on heroku. Be sure to include `{ args: ['--no-sandbox'] }` in your call to `puppeteer.launch`

## Usage

To use the latest stable version from source code in this repository:

```sh-session
heroku buildpacks:set https://github.com/fraol0912/puppeteer-heroku-buildpack.git
```

## Issues

A common issue that people run into often is a cache issue with heroku. Often when you start seeing errors that chrome won't start and some libraries are missing, you can resolve it by clearing your heroku cache. Instructions for that can be found [here](https://help.heroku.com/18PI5RSY/how-do-i-clear-the-build-cache).

If you are still running into any issues with this buildpack after doing the above, please open an issue on this repo and/or submit a PR that resolves it. Different versions of chrome have different dependencies and so some issues can creep in without me knowing. Thanks!
