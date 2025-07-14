

- StoreKit Test
- SKTestTransaction
-  pendingAskToBuyConfirmation 

Instance Property

# pendingAskToBuyConfirmation

A Boolean value that indicates whether the transaction is awaiting an Ask to Buy confirmation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var pendingAskToBuyConfirmation: Bool { get }
```

## Discussion

To test an Ask to Buy scenario, first set askToBuyEnabled to `true` before making a purchase. If pendingAskToBuyConfirmation is `true`, approve the transaction by calling approveAskToBuyTransaction(identifier:) , or decline it by calling declineAskToBuyTransaction(identifier:).

## See Also

### Getting Test Environment States

var autoRenewingEnabled: Bool

A Boolean value that indicates whether automatic renewal is enabled for the subscription.

var hasPurchaseIssue: Bool

A Boolean value that indicates whether you resolve this transaction using the test framework functions.

var isPendingPriceIncreaseConsent: Bool

A Boolean value that indicates whether the auto-renewable subscription has a price increase that’s awaiting user consent in the test environment.

