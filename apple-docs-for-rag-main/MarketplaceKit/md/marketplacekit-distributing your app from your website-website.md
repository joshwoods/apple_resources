

- MarketplaceKit
-  Distributing your app from your website 

Article

# Distributing your app from your website

Configure your app and website to enable people to install your app on their devices from your website.

## Overview

In eligible regions, you can distribute approved, non-marketplace apps from your website. To distribute your app, fill out a webform that outlines the qualifications, and if approved, Apple enables you to download a framework that facilitates the secure installation of your app from your website.

Coordinate with App Store Connect by providing your web domain and a public key that the system uses to validate your app’s installations. When you submit your app and pass review, App Store Connect enables you to access your approved app’s alternative distribution package. For more information, see Submit for Notarization.

Deploy a web server and modify your website to link to your app, which you host on your server. To prepare your app for installation, download and assemble a complete alternative distribution package using the ID that App Store Connect provides; see Ingesting an alternative distribution package. Add a Download button on your webpage that links to the alternative distribution package. The URL you assign the button uses a custom scheme that browsers handle differently, instructing them to provide the system with your app’s alternative distribution pacakge for installation on the device.

Availability

Alternative app marketplaces are available in Xcode 15.3, iOS 17.4 and later, and iPadOS 18.0 and later. To enable web distribution of other apps, use Xcode 15.4 or later, iOS 17.5 or later, and iPadOS 18.0 or later. For more information, see Xcode support.

## Request approval to distribute your app

Each app follows the same process for alternative distribution over the web and is subject to Apple’s approval, however the approval process varies by app type.

For marketplace apps, see Getting started as an alternative app marketplace in the European Union. For other apps, see Getting started with Web Distribution in the EU. In either case, you sign the Alternative EU Terms Addendum to the Developer Program License Agreement.

The signed addendum prompts App Store Connect to provide an *alternative distribution package* for your app in App Store Connect. You host this alternative distribution package on your website and use it to install your app on devices.

## Set up your app for alternative distribution

Distributing your app on the web requires one-time setup with App Store Connect. First, define the domain where you distribute the app by calling the `alternativeDistributionDomains` endpoint:

```
POST https://api.appstoreconnect.apple.com/v1/alternativeDistributionDomains
```

For more information about the request’s parameters, see Add an alternative distribution domain.

Then, supply a public key that App Store Connect uses to verify installation requests for your app by calling the `alternativeDistributionKeys` endpoint:

```
POST https://api.appstoreconnect.apple.com/v1/alternativeDistributionKeys
```

For steps to create your distribution key, see Creating keys and establishing alternative marketplace connections.

If you’re developing an alternative marketplace app, create one distribution key pair and reuse it across all your developer relationships and apps that install from your marketplace. Otherwise, create a distribution key pair for each app that you distribute from your website.

For more information about setting up a marketplace app in App Store Connect, see Create a marketplace app.

## Submit your app and host it on your web server

When you’re ready to distribute your app, submit it to App Store Connect for review. Choose the review type:

App Store  
A web-distributed binary that you also intend to release on marketplace apps, including the App Store.

Notarization  
A marketplace app or other app that won’t also reside on the App Store; see Submit for Notarization.

If Apple approves your app for distribution, download your app’s *alternative distribution package* from App Store Connect, this package contains everything that the system needs to install your app. For more information, see Get an alternative distribution package ID.

Assemble and host the alternative distribution package on your web server in a location accessible to the device; see Ingesting an alternative distribution package. When you want to update your app, submit it to App Store Connect and repeat the process.

## Add a Download button on your webpage

People download your app by tapping a button on your webpage with a URL scheme reserved for app installations. The browser forwards the installation request to the system, which retrieves the right app variant or delta from the alternative distribution package for the app that you host on your server.

The button URL is of the MarketplaceKitURIScheme format, which provides the system with everything it needs to install the app:

```
```

The URL parameters are:

| URL parameter | Description |
|----|----|
| `alternativeDistributionPackage` | Your app’s alternative distribution package. This value has unique domain-matching requirements; for more information, see MarketplaceKitURIScheme. |
| `installVerificationToken` | A required JSON web signature (JWS). For more information, see Supplying an install verification token. |
| `token` | An optional authentication token to include if downloads require authorization. The device sends the token back to your token endpoint to reference this request. The value is free-form, and can contain any information at your discretion, such as a customer identifier. |
| `account` | An optional user ID for the page visitor. The system groups apps in restore requests based on `account`. The system also provides the `account` as `login_hint` in the call to your authorization endpoint during re-authentication; for more information, see Reauthenticating a person to manage apps. |
| `appShareURL` | An optional URL to a product landing page for the app on your marketplace website. The operating system populates the value in the Share Sheet when a person touches and holds the app’s icon on the Home Screen. |

The system enforces the following criteria for a webpage that invokes an app download request:

- Your webpage initiates app installation only on a person’s express invocation; in other words, no automatic or indirect app installation. Your webpage can only install an app when a person requests it by tapping a button.

- The origin of the main frame on the webpage containing the installation link must match the domain passed to App Store Connect. The browser app records this information and sends it to MarketplaceKit as covered in Enabling alternative distribution app installation in a browser.

Tip

Some apps that Apple approves for web distribution can also install from the App Store or an alternative app marketplace. You can customize the user experience depending on the source from which a person downloads your app. For more information, see Customize your app depending on the installation source.

## Coordinate with the device from your web server

When a page visitor taps the install button, the system communicates with your web server to validate the request and retrieve the data necessary to perform the installation. If you supply an authentication token in the installation request URL, the system checks if your authentication server authorizes the download. Then system then requests an app license from your server followed by the app itself. For more information, see Installing your app from your website.

## Test your app during development

Your app can install over the web only after passing Notarization. To test your app beforehand, set the installation source for development builds. Setting the installation source enables you to simulate a web distribution in production.

Set your target’s Alternative Distribution - Web build setting to `Yes`:

Note

The build setting is `ALTERNATIVE_DISTRIBUTION_WEB`. Open your Xcode project in Xcode 15.4 or later and add the setting manually if it isn’t present.

This build setting overrides the current property for development builds to return AppDistributor.web, which enables you to test any custom code branching your app might do, such as displaying a different image or offering different menu items depending on whether your app installs from the web or a marketplace.

In your scheme’s Run task Options tab, Distribution selection menu, choose Website to simulate installation over the web for runs on device through Xcode.

Similarly, to return `web` for the `current` distributor in a test plan, choose Website in the Distribution selection menu of your test plan’s configuration.

## See Also

### Essentials

Creating an alternative app marketplace

Enable the distribution of other third-party apps from within your marketplace app.

Distributing your app on an alternative app marketplace

Design your app for alternative distribution from an alternative app marketplace.

