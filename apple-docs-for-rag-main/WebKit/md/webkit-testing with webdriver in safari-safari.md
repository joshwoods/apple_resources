

- WebKit
-  Testing with WebDriver in Safari 

Article

# Testing with WebDriver in Safari

Enable WebDriver and run a test.

## Overview

This article walks you through the process of setting up WebDriver and running a test written in Python. When a test calls a command, the command is executed in the following steps:

1.  The client library translates each command into a REST API command.

2.  The REST API command sends the corresponding HTTP request to a local web server hosted by Safari’s driver.

3.  The driver validates the HTTP request’s contents and forwards the command to the appropriate browser instance.

4.  When a command has finished executing, the driver sends an HTTP response for the REST API command. The client library interprets the HTTP response and returns the result to the test code.

### Make Sure You Have Safari’s WebDriver

Safari and Safari Technology Preview each provide their own `safaridriver` executable. Make sure you already have the executable on your device:

- Safari’s executable is located at `/usr/bin/safaridriver`.

- Safari Technology Preview’s executable is part of the application bundle’s contents.

Each `safaridriver` is capable of launching only the Safari version it’s associated with, and the two can run simultaneously. Although you can launch `safaridriver` manually by running a `safaridriver` executable, most Selenium libraries launch the driver automatically. See the documentation for your preferred client library to learn how to specify which browser to use.

### Get the Correct Selenium Library Version

Grab a recent release of the Selenium open source project. Selenium’s Java and Python client libraries offer support for Safari’s native driver implementation starting in the 3.0.0-beta1 release.

Important

Don’t use the old SafariDriver implementation, which is no longer supported by the Selenium project. The Apple-developed driver is a replacement for the legacy SafariDriver formerly maintained by the Selenium project.

### Configure Safari to Enable WebDriver Support

Safari’s WebDriver support for developers is turned off by default. How you enable it depends on your operating system.

**High Sierra and later:**

Run `safaridriver --enable` once. (If you’re upgrading from a previous macOS release, you may need to use `sudo`.)

**Sierra and earlier:**

1.  If you haven’t already done so, make the Develop menu available. Choose Safari \> Preferences, and on the Advanced tab, select “Show Develop menu in menu bar.” For details, see Safari Help.

2.  Choose Develop \> Allow Remote Automation.

3.  Authorize `safaridriver` to launch the XPC service that hosts the local web server. To permit this, manually run `/usr/bin/safaridriver` once and follow the authentication prompt.

### Write a WebDriver Testing Suite

Once you’ve obtained a client library, you can write a WebDriver test and run it against Safari. The example below uses using Python WebDriver to test important functionality of the WebKit Feature Status page.

Note

In the Python WebDriver library, each method call synchronously blocks processes until the operation completes. Other WebDriver libraries may provide an asynchronous API.

```
```

### Run Your Test

Copy and save the test code above as `test_webkit.py` and run the following:

```
```

## See Also

### WebDriver

macOS WebDriver Commands for Safari 11.1 and earlier

Test your web content using the WebDriver commands supported by Safari 11.1 and earlier.

macOS WebDriver Commands for Safari 12 and later

Test your web content using the WebDriver commands supported by Safari 12 and later.

About WebDriver for Safari

Enhance testing of your web content using Safari’s enhancements to WebDriver.

