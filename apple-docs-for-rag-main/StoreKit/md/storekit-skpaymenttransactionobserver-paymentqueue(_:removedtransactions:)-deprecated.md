

- StoreKit
- SKPaymentTransactionObserver
-  paymentQueue(\_:removedTransactions:) Deprecated

Instance Method

# paymentQueue(\_:removedTransactions:)

Tells an observer that one or more transactions have been removed from the queue.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
optional func paymentQueue(
    _ queue: SKPaymentQueue,
    removedTransactions transactions: [SKPaymentTransaction]
)
```

Deprecated

Use StoreKit 2 Transaction APIs

## Parameters 

`queue`  

The payment queue that updated the transactions.

`transactions`  

An array of the transactions that were removed.

## Mentioned in 

Processing a transaction

## Discussion

Your application does not typically need to implement this method but might implement it to update its own user interface to reflect that a transaction has been completed.

## See Also

### Handling transactions

func paymentQueue(SKPaymentQueue, updatedTransactions: [SKPaymentTransaction])

Tells an observer that one or more transactions have been updated.

**Required**

Deprecated

