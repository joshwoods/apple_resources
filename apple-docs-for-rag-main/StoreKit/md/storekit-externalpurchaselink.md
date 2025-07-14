

- StoreKit
-  ExternalPurchaseLink 

Enumeration

# ExternalPurchaseLink

Enables qualifying apps to offer external purchase links.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
enum ExternalPurchaseLink
```

## Overview

This functionality is only available to and required by apps with the com.apple.developer.storekit.external-purchase-link entitlement. For more information, see:

- Using alternative payment options on the App Store in the European Union

- Distributing dating apps in the Netherlands

- Distributing apps in Russia that provide an external purchase link

- Distributing apps in the U.S. that provide an external purchase link

- Distributing music streaming apps in the EEA that provide an external purchase link

Note

If your app is running on iOS 15.4 through 17.3 or iPadOS 15.4 through 17.3 and is configured to use the External Purchase API, you must check canMakePayments before calling the External Purchase APIs. If canMakePayments is `false`, do not call the ExternalPurchaseLink or ExternalPurchase APIs.

## Topics

### Getting multiple external purchase links

SKExternalPurchaseMultiLink

A dictionary that contains an array of URLs to websites where people using your app can make external purchases.

static var eligibleURLs: [URL]?

An array of external purchase links for the current storefront that the app configured and from which it chooses.

static func open(url: URL) async throws

Presents a continuation sheet that enables people to choose whether your app shows the indicated URL link for external purchases.

### Getting a single external purchase link

SKExternalPurchaseLink

A dictionary that contains URLs to websites where people using your app can make external purchases for supported regions.

static var canOpen: Bool

A Boolean value that indicates whether the app can successfully open the configured external purchase link in the current App Store storefront.

static func open() async throws

Presents a continuation sheet that enables people to choose whether your app shows its link for external purchases.

## Relationships

### Conforms To

- Sendable

## See Also

### Offering external purchase links

com.apple.developer.storekit.external-purchase-link

A Boolean value that indicates whether your app can include a link that directs people to a website to make an external purchase.

SKExternalPurchaseMultiLink

A dictionary that contains an array of URLs to websites where people using your app can make external purchases.

SKExternalPurchaseLink

A dictionary that contains URLs to websites where people using your app can make external purchases for supported regions.

