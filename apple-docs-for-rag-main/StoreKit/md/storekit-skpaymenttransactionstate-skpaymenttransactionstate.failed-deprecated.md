

- StoreKit
- SKPaymentTransactionState
-  SKPaymentTransactionState.failed Deprecated

Case

# SKPaymentTransactionState.failed

A failed transaction.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
case failed
```

Deprecated

Use PurchaseResult from Product.purchase(confirmIn:options:)

## Mentioned in 

Processing a transaction

Implementing promotional offers in your app

Testing In-App Purchases in Xcode

Testing an interrupted purchase

## Discussion

Check the error property to determine what happened.

## See Also

### Constants

case purchasing

A transaction that is being processed by the App Store.

Deprecated

case purchased

A successfully processed transaction.

Deprecated

case restored

A transaction that restores content previously purchased by the user.

Deprecated

case deferred

A transaction that is in the queue, but its final status is pending external action such as Ask to Buy.

Deprecated

