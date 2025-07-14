

- StoreKit Test
- SKTestTransaction
-  hasPurchaseIssue 

Instance Property

# hasPurchaseIssue

A Boolean value that indicates whether you resolve this transaction using the test framework functions.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var hasPurchaseIssue: Bool { get }
```

## Discussion

To test interrupted purchases, first set interruptedPurchasesEnabled to `true` before making a purchase. If hasPurchaseIssue value is `true`, then resolve the identified transaction by calling resolveIssueForTransaction(identifier:).

## See Also

### Getting Test Environment States

var autoRenewingEnabled: Bool

A Boolean value that indicates whether automatic renewal is enabled for the subscription.

var isPendingPriceIncreaseConsent: Bool

A Boolean value that indicates whether the auto-renewable subscription has a price increase that’s awaiting user consent in the test environment.

var pendingAskToBuyConfirmation: Bool

A Boolean value that indicates whether the transaction is awaiting an Ask to Buy confirmation.

