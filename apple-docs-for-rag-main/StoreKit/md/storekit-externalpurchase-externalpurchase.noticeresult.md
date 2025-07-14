

- StoreKit
- ExternalPurchase
-  ExternalPurchase.NoticeResult 

Enumeration

# ExternalPurchase.NoticeResult

The options available to people while viewing the external purchase notice sheet.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
enum NoticeResult
```

## Overview

These values return when your app calls presentNoticeSheet().

## Topics

### Getting notice sheet results

case cancelled

Describes when people chose to cancel and not view external purchases.

case continuedWithExternalPurchaseToken(token: String)

Describes when people chose to continue to view external purchases, and provides the external purchase token.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Offering an external purchase

static var canPresent: Bool

A Boolean value that indicates whether the app can successfully present the notice sheet to inform people about external purchases.

static func presentNoticeSheet() async throws -> ExternalPurchase.NoticeResult

Presents a notice sheet from Apple that informs people before showing external purchases and determines whether your app can present external purchases.

SKExternalPurchase

A string array of country codes that indicates your app supports external purchases.

