

- MarketplaceKit
-  Distributing your app on an alternative app marketplace 

Article

# Distributing your app on an alternative app marketplace

Design your app for alternative distribution from an alternative app marketplace.

## Overview

To distribute your app from an alternative app marketplace, review and sign the Alternative EU Terms Addendum to the Developer Program License Agreement.

Apps that reside on alternative marketplaces need to support iPhone or iPad, alternative app marketplaces don’t support other platforms. In addition, when App Store Connect sends your app to an alternative marketplace, it excludes any watchOS extensions or watch apps.

Apps on an alternative marketplace aren’t required to use MarketplaceKit. But you need to build your app with Xcode 14.1 or later and set the deployment target greater than or equal to the earliest version of iOS or iPadOS that Xcode 14.1 supports. If your app does call MarketplaceKit methods, build your app with Xcode 15.3 or later.

## Customize your app depending on the installation source

If your app installs from more than one source, you can implement conditional code to do something different, such as displaying a different graphic, depending on the source from which a person installs your app. Use MarketplaceKit app distributor’s static current property to determine the installation source:

| App distributor | Installation source |
|----|----|
| AppDistributor.appStore | The App Store |
| AppDistributor.testFlight | TestFlight |
| AppDistributor.marketplace(_:) | Alternative app marketplace; the argument `String` identifies the marketplace bundle ID |
| AppDistributor.web | The developer’s website |
| AppDistributor.other | Enterprise or education developer programs |

In apps that people install from alternative marketplaces, use APIs that vary from apps on the App Store. Specifically, use:

- AdAttributionKit for ads

- A custom e-commerce solution

- A social gaming network other than Game Center unless your app is also on the App Store

- Background Assets to download large files in the background

Don’t use StoreKit, the App Store’s In-App Purchase system, or On Demand Resources in apps you distribute outside of the App Store.

## Enable your app to run on other platforms

Apps can run on platforms that MarketplaceKit doesn’t support, including macOS using Mac Catalyst or *as-is* on Apple silicon, and visionOS. To check the platform, use `#if canImport(MarketplaceKit)`, which returns `false` for Mac apps built with Mac Catalyst and visionOS. Avoid importing MarketplaceKit on unsupported platforms, as follows:

```
```

If your app uses AppDistributor, check the platform first and avoid accessing MarketplaceKit on unsupported platforms. The following example uses `#if canImport(MarketplaceKit)` again to conditionalize access to AppDistributor:

```
```

To check for *as-is* apps that run on Apple silicon, use `ProcessInfo.processInfo.isiOSAppOnMac`:

```
```

## Establish a marketplace relationship and enable notifications

To distribute your app on a particular alternative app marketplace, contact the marketplace directly and it provides you with a unique ID that you upload to App Store Connect. Apple verifies the ID with the marketplace’s public key to confirm your agreement, or *relationship*. For more information, see Manage distribution on an alternative app marketplace.

When you’re ready to submit your app for review, choose the Notarization review type; see Submit for Notarization. app completes *Notarization*, your app becomes available for the marketplace to distribute. App Store Connect provides your Notarization-approved app in the form of an *alternative distribution package*. The package contains instructions that the alternative app marketplace follows to assemble an installable version of your app. You can download the alternative distribution package and provide it to the marketplace manually or, enable notifications in App Store Connect, which sends the package to the marketplace automatically. When notifications are on, App Store Connect keeps the marketplace up-to-date on the alternative distribution packages for all your latest app versions.

## Test your app during development

Your app can install from an alternative marketplace app only after passing Notarization. To test your app beforehand, set the installation source for development builds. Setting the installation source enables you to simulate an installation from a marketplace in production.

Set your target’s *Alternative Distribution - Marketplaces* build setting to a list of marketplace bundle IDs for the alternative marketplaces from which your app can install.

Note

The build setting by name is `MARKETPLACES`. Open your Xcode project in Xcode 15.3 or later and add the build setting manually if one by that title isn’t present.

This build setting overrides the current property for development builds, which enables you to test any custom code branching your app might do, such as displaying a different image or offering different menu items.

In your scheme’s Run task Options tab, Distribution selection menu, choose that marketplace’s bundle ID to simulate installation from that marketplace for runs on device through Xcode.

Similarly, to override the `current` distributor in a test plan, choose a marketplace bundle ID in the Distribution selection menu of your test plan’s configuration.

## See Also

### Essentials

Creating an alternative app marketplace

Enable the distribution of other third-party apps from within your marketplace app.

Distributing your app from your website

Configure your app and website to enable people to install your app on their devices from your website.

