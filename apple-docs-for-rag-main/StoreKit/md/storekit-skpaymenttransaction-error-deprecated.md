

- StoreKit
- SKPaymentTransaction
-  error Deprecated

Instance Property

# error

An object describing the error that occurred while processing the transaction.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var error: (any Error)? { get }
```

Deprecated

Use PurchaseResult from Product.purchase(confirmIn:options:)

## Discussion

The error property is undefined except when transactionState is set to SKPaymentTransactionState.failed. Your application can read the error property to determine why the transaction failed. For a list of error constants, see SKErrorDomain in `StoreKit Constants`.

## See Also

### Related Documentation

In-App Purchase Programming Guide

### Getting Transaction Information

var payment: SKPayment

The payment for the transaction.

Deprecated

var transactionIdentifier: String?

A string that uniquely identifies a successful payment transaction.

Deprecated

var transactionDate: Date?

The date the transaction was added to the App Store’s payment queue.

Deprecated

var original: SKPaymentTransaction?

The transaction that was restored by the App Store.

Deprecated

var transactionReceipt: Data?

A signed receipt that records all information about a successful payment transaction.

Deprecated

