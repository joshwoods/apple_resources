

- MarketplaceKit
-  Enabling alternative distribution app installation in a browser 

Article

# Enabling alternative distribution app installation in a browser

Add support for browser apps to install alternative distribution apps from websites.

## Overview

To enable the installation of an alternative distribution app from a webpage, your browser listens for installation requests from the website visitor’s interaction with the page and hands off the request to MarketplaceKit. The installation request uses a specific URL scheme (MarketplaceKitURIScheme) that the marketplace page assigns to a button. MarketplaceKit handles the request by presenting the app install sheet, in which the person can confirm and install the alternative distribution app on their device.

MarketplaceKit requires a one-to-one mapping between an alternative distribution app and the domain of the website that distributes it. When a page visitor taps a button to install the app, your browser app passes the origin of the site’s main frame to MarketplaceKit, which confirms that the owner of the domain also owns the app.

Note

The system requires that your browser app have a specific entitlement to call the MarketplaceKit installation method. For more information and to request the entitlement, see com.apple.developer.browser.app-installation.

## Respond to app installation requests using BrowserEngineKit

Browsers that render using BrowserEngineKit hand off app installation requests to MarketplaceKit. Your browser listens for invocations to a URL with the scheme `MarketplaceKit/MarketplaceKitURIScheme`:

```
marketplace-kit://install
    ?alternativeDistributionPackage=
    &installVerificationToken=
    &token=
    &account=
    &appShareURL=;
```

The URL parameters are:

| URL parameter | Description |
|----|----|
| `alternativeDistributionPackage` | The app to install in the form of an alternative distribution package. |
| `installVerificationToken` | A required JSON web signature (JWS). |
| `token` | An optional authentication token. |
| `account` | An optional user ID for the page visitor. |
| `appShareURL` | An optional URL to a product landing page for the app on the marketplace website. |

For more information about the parameters, see MarketplaceKitURIScheme.

To forward the navigation request to MarketplaceKit, call the requestAppInstallationFromBrowser(for:referrer:) method to display the app install sheet and pass in the following parameters:

| URL parameter | Description |
|----|----|
| `url` | The unparsed MarketplaceKitURIScheme URL that triggers the installation request. |
| `referrer` | The origin of the main frame that contains the alternative marketplace installation URL. |

Important

To comply with operation system requirements, ignore the `marketplace-kit://` URL invocation if the navigation doesn’t result from a user interaction, such as tapping a button, or if the navigation results from a redirect.

## Respond to app installation requests using WebKit

If your browser app uses WebKit, modify your app’s webView(_:decidePolicyFor:decisionHandler:) navigation delegate method. When the system calls the delegate method with a URL matching the `MarketplaceKitURIScheme` scheme, call the `decisionHandler` with a value of `WKNavigationActionPolicyAllow`.

Don’t call the requestAppInstallationFromBrowser(for:referrer:) method directly. WebKit handles the interaction with MarketplaceKit after you call the navigation delegate’s `decisionHandler` with a value of `WKNavigationActionPolicyAllow`.

Safari is an example of a browser app that uses WebKit. When a person taps on an `MarketplaceKitURIScheme` URL, it calls Safari’s webView(_:decidePolicyFor:decisionHandler:) navigation delegate method with a URL matching the `MarketplaceKitURIScheme`. Safari responds by calling `decisionHandler` with `WKNavigationActionPolicyAllow`, which then causes WebKit to pass the URL to MarketplaceKit and display an install sheet.

## Test web distribution during development

In iOS or iPadOS 18.2 and later, development builds of browser apps with the default browser entitlement (com.apple.developer.web-browser) can test the installation of app marketplaces and other apps that distribute over the web. A development build signed with a development or Ad Hoc provisioning profile can run on Simulator and all supported physical devices (iPhone and iPad).

