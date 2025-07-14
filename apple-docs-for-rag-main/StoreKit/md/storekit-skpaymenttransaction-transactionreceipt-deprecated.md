

- StoreKit
- SKPaymentTransaction
-  transactionReceipt Deprecated

Instance Property

# transactionReceipt

A signed receipt that records all information about a successful payment transaction.

tvOSDeprecated

``` source
var transactionReceipt: Data? { get }
```

Deprecated

Use the app receipt instead, as described in Receipt Validation Programming Guide.

## Discussion

The contents of this property are undefined except when transactionState is set to SKPaymentTransactionState.purchased.

The receipt is a signed chunk of data that can be sent to the App Store to verify that the payment was successfully processed. This is most useful when designing a store that uses a server separate from the iPhone to verify that payment was processed. For more information on verifying receipts, see Receipt Validation Programming Guide.

## See Also

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

var error: (any Error)?

An object describing the error that occurred while processing the transaction.

Deprecated

