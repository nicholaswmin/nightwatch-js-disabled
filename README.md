# Run [NightwatchJS][nightwatchJS] tests with javascript disabled

Sample project for this [S.O answer][SO-answer]

## Install

### Clone/Install

```bash
$ git clone https://github.com/nicholaswmin/nightwatch-js-disabled
$ cd nightwatch-js-disabled
$ npm install
```

### Install NightwatchJS

```bash
$ npm install -g nightwatch
```

### Run selenium server

```bash
$ java -jar selenium/selenium-server-standalone-3.9.1.jar
```

### Run the tests

```bash
$ nightwatch test.js
```

The above will run the test file, `test.js` which basically visits
https://stackoverflow.com with JS disabled and verifies that it shows
the "JavaScript Disabled" warning.

The configuration that hints to WebDriver that it should start Chromium
with JS disabled is in `nightwatch.json` in the root directory.

The tests only run on Chrome, but you can add other browsers/configuration
if you want to by visiting [NightwatchJS Getting Started][nightwatchJS].

## License

MIT

[nightwatchJS]: http://nightwatchjs.org/gettingstarted
[SO-answer]: https://stackoverflow.com/a/52806859/1814486
