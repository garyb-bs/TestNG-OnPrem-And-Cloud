# TestNG On Prem and Cloud Implementation

[TestNG](http://testng.org) Integration with BrowserStack and On Prem

![BrowserStack Logo](https://d98b8t1nnulk5.cloudfront.net/production/images/layout/logo-header.png?1469004780)

## Using Maven

### Setup

* Clone the repo
* Install dependencies `mvn compile`
* Update `*.conf.json` files inside the `src/test/resources/conf` directory with your [BrowserStack Username and Access Key](https://www.browserstack.com/accounts/settings)

### Running your tests

- To run a single test on BrowserStack, run
 ```
 mvn test -P single 
 ```
- To run tests on your local sites using BrowserStack, run 
```
 mvn test -P local 
 ```
- To run tests on parallel devices on BrowserStack, run
```
 mvn test -P parallel 
 ```
- To run the tests using a WebDriver on your machine, run
```
 mvn test -P on-prem
 ```

## Notes
* You can view your test results on the [BrowserStack Automate dashboard](https://www.browserstack.com/automate)
* To test on a different set of browsers, check out our [platform configurator](https://www.browserstack.com/automate/java#setting-os-and-browser)
* You can export the environment variables for the Username and Access Key of your BrowserStack account

  ```
  export BROWSERSTACK_USERNAME=<browserstack-username> &&
  export BROWSERSTACK_ACCESS_KEY=<browserstack-access-key>
  ```

## Additional Resources
* [Documentation for writing Automate test scripts in Java](https://www.browserstack.com/automate/java)
* [Customizing your tests on BrowserStack](https://www.browserstack.com/automate/capabilities)
* [Browsers & mobile devices for selenium testing on BrowserStack](https://www.browserstack.com/list-of-browsers-and-platforms?product=automate)
* [Using REST API to access information about your tests via the command-line interface](https://www.browserstack.com/automate/rest-api)
