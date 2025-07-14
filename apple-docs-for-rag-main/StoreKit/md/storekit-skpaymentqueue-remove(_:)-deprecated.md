

- StoreKit
- SKPaymentQueue
-  remove(\_:) Deprecated

Instance Method

# remove(\_:)

Removes an observer from the payment queue.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
func remove(_ observer: any SKPaymentTransactionObserver)
```

Deprecated

No longer supported

## Parameters 

`observer`  

The observer to remove.

## Discussion

If there are no observers attached to the queue, the payment queue does not synchronize its list of pending transactions with the Apple App Store, because there is no observer to respond to updated transactions.

## See Also

### Related Documentation

var transactions: [SKPaymentTransaction]

Returns an array of pending transactions.

Deprecated

### Adding, Getting, and Removing Observers

func add(any SKPaymentTransactionObserver)

Adds an observer to the payment queue.

Deprecated

var transactionObservers: [any SKPaymentTransactionObserver]

An array of all active payment queue observers.

Deprecated

