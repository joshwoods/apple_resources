

- StoreKit
- SKPaymentTransaction
-  transactionIdentifier Deprecated

Instance Property

# transactionIdentifier

A string that uniquely identifies a successful payment transaction.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var transactionIdentifier: String? { get }
```

Deprecated

Use PurchaseResult from Product.purchase(confirmIn:options:)

## Discussion

The contents of this property are undefined except when transactionState is set to SKPaymentTransactionState.purchased or SKPaymentTransactionState.restored. The transactionIdentifier is a string that uniquely identifies an interaction between the user’s device and the App Store, such as a purchase or restore.

This value has the same format as the transaction’s transaction_id in the receipt; however, the values may not be the same.

## See Also

### Getting Transaction Information

var payment: SKPayment

The payment for the transaction.

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

