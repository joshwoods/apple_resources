

- StoreKit
- SKPaymentQueue
-  restoreCompletedTransactions(withApplicationUsername:) Deprecated

Instance Method

# restoreCompletedTransactions(withApplicationUsername:)

Asks the payment queue to restore previously completed purchases, providing an opaque identifier for the user’s account.

iOS 7.0–18.0DeprecatediPadOS 7.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.9–15.0DeprecatedtvOS 7.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
func restoreCompletedTransactions(withApplicationUsername username: String?)
```

Deprecated

Use AppStore.sync()

## Parameters 

`username`  

An opaque identifier for the user’s account on your system.

## Mentioned in 

Restoring purchased products

Choosing a receipt validation technique

Testing In-App Purchases in Xcode

## See Also

### Related Documentation

var applicationUsername: String?

A string that associates the transaction with a user account on your service.

Deprecated

### Restoring Purchases

func restoreCompletedTransactions()

Asks the payment queue to restore previously completed purchases.

Deprecated

