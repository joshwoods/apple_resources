

- StoreKit
- SKPaymentQueue
-  transactions Deprecated

Instance Property

# transactions

Returns an array of pending transactions.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var transactions: [SKPaymentTransaction] { get }
```

Deprecated

Use Transaction.unfinished

## Discussion

The value of this property is undefined when there are no observers attached to the payment queue.

## See Also

### Related Documentation

func add(any SKPaymentTransactionObserver)

Adds an observer to the payment queue.

Deprecated

### Managing Transactions

var delegate: (any SKPaymentQueueDelegate)?

A delegate that provides information needed to complete transactions.

Deprecated

func add(SKPayment)

Adds a payment request to the queue.

Deprecated

func finishTransaction(SKPaymentTransaction)

Notifies the App Store that the app finished processing the transaction.

Deprecated

