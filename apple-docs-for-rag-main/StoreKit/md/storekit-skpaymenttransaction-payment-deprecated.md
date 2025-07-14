

- StoreKit
- SKPaymentTransaction
-  payment Deprecated

Instance Property

# payment

The payment for the transaction.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var payment: SKPayment { get }
```

Deprecated

Use PurchaseResult from Product.purchase(confirmIn:options:)

## Discussion

Each payment transaction is created in response to a payment that your application added to the payment queue.

## See Also

### Getting Transaction Information

var transactionIdentifier: String?

A string that uniquely identifies a successful payment transaction.

Deprecated

var transactionDate: Date?

The date the transaction was added to the App Store’s payment queue.

Deprecated

var original: SKPaymentTransaction?

The transaction that was restored by the App Store.

Deprecated

var error: (any Error)?

An object describing the error that occurred while processing the transaction.

Deprecated

var transactionReceipt: Data?

A signed receipt that records all information about a successful payment transaction.

Deprecated

