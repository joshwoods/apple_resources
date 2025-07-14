

- StoreKit
- SKPaymentTransactionObserver
-  paymentQueue(\_:restoreCompletedTransactionsFailedWithError:) Deprecated

Instance Method

# paymentQueue(\_:restoreCompletedTransactionsFailedWithError:)

Tells the observer that an error occurred while restoring transactions.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
optional func paymentQueue(
    _ queue: SKPaymentQueue,
    restoreCompletedTransactionsFailedWithError error: any Error
)
```

Deprecated

Use AppStore.sync()

## Parameters 

`queue`  

The payment queue that was restoring transactions.

`error`  

The error that occurred.

## Mentioned in 

Processing a transaction

## See Also

### Restoring transactions

func paymentQueueRestoreCompletedTransactionsFinished(SKPaymentQueue)

Tells the observer that the payment queue has finished sending restored transactions.

Deprecated

