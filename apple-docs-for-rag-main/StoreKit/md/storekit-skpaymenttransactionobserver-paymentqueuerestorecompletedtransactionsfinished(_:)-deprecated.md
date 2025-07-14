

- StoreKit
- SKPaymentTransactionObserver
-  paymentQueueRestoreCompletedTransactionsFinished(\_:) Deprecated

Instance Method

# paymentQueueRestoreCompletedTransactionsFinished(\_:)

Tells the observer that the payment queue has finished sending restored transactions.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
optional func paymentQueueRestoreCompletedTransactionsFinished(_ queue: SKPaymentQueue)
```

Deprecated

Use AppStore.sync()

## Parameters 

`queue`  

The payment queue that restored the transactions.

## Mentioned in 

Processing a transaction

Testing In-App Purchases in Xcode

## Discussion

This method is called after all restorable transactions have been processed by the payment queue. Your application is not required to do anything in this method.

## See Also

### Restoring transactions

func paymentQueue(SKPaymentQueue, restoreCompletedTransactionsFailedWithError: any Error)

Tells the observer that an error occurred while restoring transactions.

Deprecated

