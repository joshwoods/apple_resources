

- StoreKit
- SKPaymentQueue
-  delegate Deprecated

Instance Property

# delegate

A delegate that provides information needed to complete transactions.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.15–15.0DeprecatedtvOS 13.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
weak var delegate: (any SKPaymentQueueDelegate)? { get set }
```

Deprecated

No longer supported

## Discussion

This delegate implements the SKPaymentQueueDelegate protocol.

## See Also

### Managing Transactions

var transactions: [SKPaymentTransaction]

Returns an array of pending transactions.

Deprecated

func add(SKPayment)

Adds a payment request to the queue.

Deprecated

func finishTransaction(SKPaymentTransaction)

Notifies the App Store that the app finished processing the transaction.

Deprecated

