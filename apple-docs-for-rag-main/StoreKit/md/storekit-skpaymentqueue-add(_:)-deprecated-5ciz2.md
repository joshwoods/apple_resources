

- StoreKit
- SKPaymentQueue
-  add(\_:) Deprecated

Instance Method

# add(\_:)

Adds an observer to the payment queue.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
func add(_ observer: any SKPaymentTransactionObserver)
```

Deprecated

Use Transaction.updates or PurchaseResult from Product.purchase(confirmIn:options:)

## Parameters 

`observer`  

The observer to add to the queue.

## Mentioned in 

Choosing a receipt validation technique

Testing transaction observer code

## Discussion

Your application should add an observer to the payment queue during application initialization. If there are no observers attached to the queue, the payment queue does not synchronize its list of pending transactions with the Apple App Store, because there is no observer to respond to updated transactions.

If an application quits when transactions are still being processed, those transactions are not lost. The next time the application launches, the payment queue resumes processing the transactions. Your application should always expect to be notified of completed transactions.

If more than one transaction observer is attached to the payment queue, no guarantees are made as to the order which they will be called. It is safe for multiple observers to call finishTransaction(_:), but not recommended. It is recommended that you use a single observer to process and finish the transaction.

## See Also

### Related Documentation

var transactions: [SKPaymentTransaction]

Returns an array of pending transactions.

Deprecated

### Adding, Getting, and Removing Observers

var transactionObservers: [any SKPaymentTransactionObserver]

An array of all active payment queue observers.

Deprecated

func remove(any SKPaymentTransactionObserver)

Removes an observer from the payment queue.

Deprecated

