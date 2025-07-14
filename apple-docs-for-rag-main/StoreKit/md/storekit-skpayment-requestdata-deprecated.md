

- StoreKit
- SKPayment
-  requestData Deprecated

Instance Property

# requestData

Reserved for future use.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var requestData: Data? { get }
```

Deprecated

Create Product.PurchaseOption.custom values to use in Product.purchase(confirmIn:options:)

## Discussion

The default value is `nil`. If requestData is not `nil`, your payment request will be rejected.

## See Also

### Getting Payment Details

var productIdentifier: String

A string used to identify a product that can be purchased from within your app.

Deprecated

var quantity: Int

The number of items the user wants to purchase.

Deprecated

var applicationUsername: String?

A string that associates the transaction with a user account on your service.

Deprecated

