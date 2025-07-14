

- StoreKit
- SKPayment
-  applicationUsername Deprecated

Instance Property

# applicationUsername

A string that associates the transaction with a user account on your service.

iOS 7.0–18.0DeprecatediPadOS 7.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.9–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var applicationUsername: String? { get }
```

Deprecated

Create a Product.PurchaseOption.appAccountToken to use in Product.purchase(confirmIn:options:)

## Discussion

For more information on how to set and use this property, see applicationUsername.

## See Also

### Getting Payment Details

var productIdentifier: String

A string used to identify a product that can be purchased from within your app.

Deprecated

var quantity: Int

The number of items the user wants to purchase.

Deprecated

var requestData: Data?

Reserved for future use.

Deprecated

