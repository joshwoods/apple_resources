

- MarketplaceKit
-  AppDistributor 

Enumeration

# AppDistributor

Options that describe the marketplace from which the app installs.

iOS 17.4+iPadOS 17.4+Mac CatalystmacOS 15.0+

``` source
enum AppDistributor
```

## Mentioned in 

Distributing your app on an alternative app marketplace

## Overview

Apps on alternative app marketplaces need to use APIs that vary from apps on the App Store. Specifically, use:

- AdAttributionKit for ads.

- An e-commerce solution other than the App Store’s In-App Purchase system.

- A social gaming network other than Game Center unless your app is also on the App Store.

- Background Assets to download large files in the background rather than On Demand Resources.

Only use StoreKit on the App Store.

To observe API differences, check the value of the app distributor’s static (current) property to determine the installation source:

| App distributor case | Installation source |
|----|----|
| AppDistributor.appStore | The App Store |
| AppDistributor.testFlight | TestFlight |
| AppDistributor.marketplace(_:) | Alternative app marketplace; the argument `String` identifies the marketplace bundle ID |
| AppDistributor.web | The developer’s website |
| AppDistributor.other | Enterprise or education developer programs |

For more information, see Distributing your app on an alternative app marketplace.

## Topics

### Enumeration Cases

case appStore

case marketplace(String)

case other

case testFlight

case web

### Type Properties

static var current: AppDistributor

The source from which the app installs.

