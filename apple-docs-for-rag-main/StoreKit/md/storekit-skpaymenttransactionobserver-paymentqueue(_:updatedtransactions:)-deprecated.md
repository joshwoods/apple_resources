

- StoreKit
- SKPaymentTransactionObserver
-  paymentQueue(\_:updatedTransactions:) Deprecated

Instance Method

# paymentQueue(\_:updatedTransactions:)

Tells an observer that one or more transactions have been updated.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
func paymentQueue(
    _ queue: SKPaymentQueue,
    updatedTransactions transactions: [SKPaymentTransaction]
)
```

**Required**

Deprecated

Use StoreKit 2 Transaction APIs

## Parameters 

`queue`  

The payment queue that updated the transactions.

`transactions`  

An array of the transactions that were updated.

## Mentioned in 

Testing In-App Purchases in Xcode

Testing a successful transaction

Testing a payment request

Implementing offer codes in your app

Testing resubscribing from the subscriptions page

## Discussion

The application should process each transaction by examining the transaction’s transactionState property. If transactionState is SKPaymentTransactionState.purchased, payment was successfully received for the desired functionality. The application should make the functionality available to the user. If transactionState is SKPaymentTransactionState.failed, the application can read the transaction’s error property to return a meaningful error to the user.

Once a transaction is processed, it should be removed from the payment queue by calling the payment queue’s finishTransaction(_:) method, passing the transaction as a parameter.

Important

Once the transaction is finished, StoreKit can’t tell you that this item is already purchased. It is important that applications process the transaction completely before calling finishTransaction(_:).

## See Also

### Related Documentation

In-App Purchase Programming Guide

### Handling transactions

func paymentQueue(SKPaymentQueue, removedTransactions: [SKPaymentTransaction])

Tells an observer that one or more transactions have been removed from the queue.

Deprecated

