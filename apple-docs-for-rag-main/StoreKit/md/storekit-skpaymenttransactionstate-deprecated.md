

- StoreKit
-  SKPaymentTransactionState Deprecated

Enumeration

# SKPaymentTransactionState

Values representing the state of a transaction.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
enum SKPaymentTransactionState
```

Deprecated

Use PurchaseResult from Product.purchase(confirmIn:options:)

## Topics

### Constants

case purchasing

A transaction that is being processed by the App Store.

case purchased

A successfully processed transaction.

case failed

A failed transaction.

case restored

A transaction that restores content previously purchased by the user.

case deferred

A transaction that is in the queue, but its final status is pending external action such as Ask to Buy.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Transaction State

var transactionState: SKPaymentTransactionState

The current state of the transaction.

Deprecated

