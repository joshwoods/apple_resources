

- StoreKit
- SKPaymentTransactionState
-  SKPaymentTransactionState.deferred Deprecated

Case

# SKPaymentTransactionState.deferred

A transaction that is in the queue, but its final status is pending external action such as Ask to Buy.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.10–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
case deferred
```

Deprecated

Use PurchaseResult.pending from Product.purchase(confirmIn:options:)

## Mentioned in 

Processing a transaction

## Discussion

Update your UI to show the deferred state, and wait for another callback that indicates the final status.

## See Also

### Constants

case purchasing

A transaction that is being processed by the App Store.

Deprecated

case purchased

A successfully processed transaction.

Deprecated

case failed

A failed transaction.

Deprecated

case restored

A transaction that restores content previously purchased by the user.

Deprecated

