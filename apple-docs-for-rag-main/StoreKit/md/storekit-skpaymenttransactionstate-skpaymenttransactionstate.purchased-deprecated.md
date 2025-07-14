

- StoreKit
- SKPaymentTransactionState
-  SKPaymentTransactionState.purchased Deprecated

Case

# SKPaymentTransactionState.purchased

A successfully processed transaction.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
case purchased
```

Deprecated

Use PurchaseResult from Product.purchase(confirmIn:options:)

## Mentioned in 

Testing In-App Purchases in Xcode

Testing a successful transaction

Testing an interrupted purchase

Implementing offer codes in your app

Implementing promotional offers in your app

## Discussion

Your application should provide the content the user purchased.

## See Also

### Constants

case purchasing

A transaction that is being processed by the App Store.

Deprecated

case failed

A failed transaction.

Deprecated

case restored

A transaction that restores content previously purchased by the user.

Deprecated

case deferred

A transaction that is in the queue, but its final status is pending external action such as Ask to Buy.

Deprecated

