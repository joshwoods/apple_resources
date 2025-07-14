

- StoreKit Test
- SKTestSession
-  shouldEnterBillingRetryOnRenewal 

Instance Property

# shouldEnterBillingRetryOnRenewal

A Boolean value that indicates whether the testing environment enters a billing retry state when an auto-renewable subscription renews.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+watchOS 8.5+

``` source
var shouldEnterBillingRetryOnRenewal: Bool { get set }
```

## Discussion

The default value is `false`.

While this property is enabled, all renewals of auto-renewable subscriptions in the test environment fail due to a simulated billing issue and enter a billing retry state. To resolve the simulated billing issue, call resolveIssueForTransaction(identifier:) for the affected auto-renewable subscription.

The timeRate value determines the length of the billing retry period in the testing environment.

## See Also

### Testing billing retry and grace period

var billingGracePeriodIsEnabled: Bool

A Boolean value that indicates whether the test environment simulates a billing grace period for auto-renewable subscriptions.

func resolveIssueForTransaction(identifier: Int) throws

Simulates resolving an issue when you test interrupted purchases or billing retry scenarios.

