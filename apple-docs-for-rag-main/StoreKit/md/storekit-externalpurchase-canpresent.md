

- StoreKit
- ExternalPurchase
-  canPresent 

Type Property

# canPresent

A Boolean value that indicates whether the app can successfully present the notice sheet to inform people about external purchases.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
static var canPresent: Bool { get async }
```

## Discussion

Check this property, as shown below, to determine whether your app can successfully call presentNoticeSheet() to inform people before showing external purchases:

```
await externalPurchase.canPresent 
```

Check the value of this property again whenever the App Store storefront changes by using the updates asynchronous sequence of Storefront.

This property is `true` if all the following conditions are met:

- The current App Store storefront allows external purchase, and the person is eligible to make external purchases.

- Your app configures the com.apple.developer.storekit.external-purchase entitlement.

- Your app configures the country code for the current App Store storefront in SKExternalPurchase.

Otherwise, this property is `false`.

When this property is `false`, check canMakePayments to determine whether your app can offer in-app purchases using the StoreKit In-App Purchase APIs. For more information, see canMakePayments.

## See Also

### Offering an external purchase

static func presentNoticeSheet() async throws -> ExternalPurchase.NoticeResult

Presents a notice sheet from Apple that informs people before showing external purchases and determines whether your app can present external purchases.

enum NoticeResult

The options available to people while viewing the external purchase notice sheet.

SKExternalPurchase

A string array of country codes that indicates your app supports external purchases.

