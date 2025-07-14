

- StoreKit Test
- SKTestTransaction
-  autoRenewingEnabled 

Instance Property

# autoRenewingEnabled

A Boolean value that indicates whether automatic renewal is enabled for the subscription.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var autoRenewingEnabled: Bool { get }
```

## Discussion

By default, the system creates subscriptions with auto-renew enabled. To disable auto-renew, call disableAutoRenewForTransaction(identifier:).

## See Also

### Getting Test Environment States

var hasPurchaseIssue: Bool

A Boolean value that indicates whether you resolve this transaction using the test framework functions.

var isPendingPriceIncreaseConsent: Bool

A Boolean value that indicates whether the auto-renewable subscription has a price increase that’s awaiting user consent in the test environment.

var pendingAskToBuyConfirmation: Bool

A Boolean value that indicates whether the transaction is awaiting an Ask to Buy confirmation.

