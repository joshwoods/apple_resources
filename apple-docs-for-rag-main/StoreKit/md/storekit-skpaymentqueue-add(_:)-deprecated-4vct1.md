

- StoreKit
- SKPaymentQueue
-  add(\_:) Deprecated

Instance Method

# add(\_:)

Adds a payment request to the queue.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
func add(_ payment: SKPayment)
```

Deprecated

Use Product.purchase(confirmIn:options:)

## Parameters 

`payment`  

A payment request.

## Discussion

An application should always have at least one observer of the payment queue before adding payment requests.

The payment request must have a product identifier registered with the Apple App Store and a quantity greater than `0`. If either property is invalid, add(_:) throws an exception.

When a payment request is added to the queue, the payment queue processes that request with the Apple App Store and arranges for payment from the user. When that transaction is complete or if a failure occurs, the payment queue sends the SKPaymentTransaction object that encapsulates the request to all transaction observers.

## See Also

### Managing Transactions

var delegate: (any SKPaymentQueueDelegate)?

A delegate that provides information needed to complete transactions.

Deprecated

var transactions: [SKPaymentTransaction]

Returns an array of pending transactions.

Deprecated

func finishTransaction(SKPaymentTransaction)

Notifies the App Store that the app finished processing the transaction.

Deprecated

