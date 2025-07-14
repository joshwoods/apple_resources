

- StoreKit
- SKMutablePayment
-  productIdentifier Deprecated

Instance Property

# productIdentifier

A string that identifies a product that can be purchased from within your app.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var productIdentifier: String { get set }
```

Deprecated

Use Product.purchase(confirmIn:options:)

## Discussion

The product identifier is a string previously agreed on between your app and the Apple App Store.

## See Also

### Related Documentation

In-App Purchase Programming Guide

### Getting and Setting Attributes

var quantity: Int

The number of items the user wants to purchase.

Deprecated

var requestData: Data?

Reserved for future use.

Deprecated

var applicationUsername: String?

A string that associates the transaction with a user account on your service.

Deprecated

