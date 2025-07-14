

- StoreKit
- SKPayment
-  quantity Deprecated

Instance Property

# quantity

The number of items the user wants to purchase.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var quantity: Int { get }
```

Deprecated

Create a Product.PurchaseOption.quantity to use in Product.purchase(confirmIn:options:)

## Discussion

The default value is 1, the minimum value is 1, and the maximum value is 10.

## See Also

### Getting Payment Details

var productIdentifier: String

A string used to identify a product that can be purchased from within your app.

Deprecated

var requestData: Data?

Reserved for future use.

Deprecated

var applicationUsername: String?

A string that associates the transaction with a user account on your service.

Deprecated

