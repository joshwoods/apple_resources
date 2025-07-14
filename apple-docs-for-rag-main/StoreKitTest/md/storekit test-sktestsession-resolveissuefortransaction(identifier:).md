

- StoreKit Test
- SKTestSession
-  resolveIssueForTransaction(identifier:) 

Instance Method

# resolveIssueForTransaction(identifier:)

Simulates resolving an issue when you test interrupted purchases or billing retry scenarios.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func resolveIssueForTransaction(identifier: Int) throws
```

## Parameters 

`identifier`  

The transaction identifier for the transaction that the test environment resolves.

## Discussion

Call this method to simulate a user resolving an issue that prevents a purchase, such as an interrupted purchase or a billing issue. You enable the testing environment to simulate the issues by setting the interruptedPurchasesEnabled and billingGracePeriodIsEnabled properties, respectively.

In the production environment, users resolve the issues by completing actions outside of your app. For example, users may need to agree to new terms and conditions or update a payment card.

When you call resolveIssueForTransaction(identifier:), your app receives the new transaction in the updates sequence or the transactionObservers.

## See Also

### Testing interrupted purchases

var interruptedPurchasesEnabled: Bool

A Boolean value that determines whether the test environment simulates an interrupted purchase.

