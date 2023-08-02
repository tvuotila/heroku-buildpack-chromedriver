# heroku-buildpack-chromedriver

This buildpack installs
[`chromedriver`](https://chromedriver.chromium.org/)
 (the Selenium driver for Chrome) in a Heroku slug.
 
 This buildpack only installs the `chromedriver` binary. To use Selenium with Chrome
 on Heroku, you'll also need Chrome. We suggest one of these buildpacks:
 
 - [heroku-buildpack-google-chrome](https://github.com/tvuotila/heroku-buildpack-google-chrome)
   to run Chrome with the `--headless` flag


## Configuring the downloaded version of chromedriver.

This buildpack will download the latest release, which is provided
by [Chrome for testing](https://googlechromelabs.github.io/chrome-for-testing/last-known-good-versions-with-downloads.json).


## Releasing a new version

Make sure you publish this buildpack in the buildpack registry

`heroku buildpacks:publish heroku/chromedriver master`
