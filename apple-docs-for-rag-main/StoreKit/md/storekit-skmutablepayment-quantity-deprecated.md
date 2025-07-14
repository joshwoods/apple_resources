

- StoreKit
- SKMutablePayment
-  quantity Deprecated

Instance Property

# quantity

The number of items the user wants to purchase.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var quantity: Int { get set }
```

Deprecated

Create a Product.PurchaseOption.quantity to use in Product.purchase(confirmIn:options:)

## Discussion

The quantity property must be greater than `0`.

## See Also

### Getting and Setting Attributes

var productIdentifier: String

A string that identifies a product that can be purchased from within your app.

Deprecated

var requestData: Data?

Reserved for future use.

Deprecated

var applicationUsername: String?

A string that associates the transaction with a user account on your service.

Deprecated

