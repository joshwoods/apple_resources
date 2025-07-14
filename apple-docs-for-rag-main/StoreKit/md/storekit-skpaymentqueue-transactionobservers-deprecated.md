

- StoreKit
- SKPaymentQueue
-  transactionObservers Deprecated

Instance Property

# transactionObservers

An array of all active payment queue observers.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var transactionObservers: [any SKPaymentTransactionObserver] { get }
```

Deprecated

Use Transaction.updates or PurchaseResult from Product.purchase(confirmIn:options:)

## See Also

### Adding, Getting, and Removing Observers

func add(any SKPaymentTransactionObserver)

Adds an observer to the payment queue.

Deprecated

func remove(any SKPaymentTransactionObserver)

Removes an observer from the payment queue.

Deprecated

