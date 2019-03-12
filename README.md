# containerized-angular

## Angular tests 

In order to execute tests within container you need to modify the karma.conf.js as following:

```
browsers: ['ChromeHeadlessNoSandbox'],
customLaunchers: {
  ChromeHeadlessNoSandbox: {
    base: 'ChromeHeadless',
    flags: ['--no-sandbox']
  }
}
```
