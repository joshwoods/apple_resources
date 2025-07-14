

- StoreKit
-  ExternalPurchase 

Enumeration

# ExternalPurchase

Enables qualifying apps to offer external purchases within the app.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
enum ExternalPurchase
```

## Overview

This functionality is only available to and required by apps with the com.apple.developer.storekit.external-purchase entitlement. For more information, see:

- Distributing apps using alternative payment providers in the European Union

- Distributing dating apps in the Netherlands

- Distributing apps using a third-party payment provider in South Korea

Note

If your app is running on iOS 15.4 through 17.3 or the iPadOS 15.4 through 17.3 and configured to use the External Purchase API, you must check canMakePayments before calling the External Purchase APIs. If canMakePayments is `false`, do not call the ExternalPurchaseLink or ExternalPurchase APIs.

## Topics

### Offering an external purchase

static var canPresent: Bool

A Boolean value that indicates whether the app can successfully present the notice sheet to inform people about external purchases.

static func presentNoticeSheet() async throws -> ExternalPurchase.NoticeResult

Presents a notice sheet from Apple that informs people before showing external purchases and determines whether your app can present external purchases.

enum NoticeResult

The options available to people while viewing the external purchase notice sheet.

SKExternalPurchase

A string array of country codes that indicates your app supports external purchases.

## Relationships

### Conforms To

- Sendable

## See Also

### Offering external purchases

com.apple.developer.storekit.external-purchase

A Boolean value that indicates whether your app can offer external purchases.

SKExternalPurchase

A string array of country codes that indicates your app supports external purchases.

