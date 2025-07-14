

- StoreKit Test
- SKTestSession
-  timeRate 

Instance Property

# timeRate

The rate at which time passes for subscriptions in the test environment as compared to real time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var timeRate: SKTestSession.TimeRate { get set }
```

## Discussion

Use the timeRate value when you test auto-renewable subscriptions to speed up or slow down the time it takes for subscriptions to renew in the test environment. The default value is SKTestSession.TimeRate.realTime. For maximum accelerated time, use SKTestSession.TimeRate.oneRenewalEveryTwoSeconds.

To test subscription renewals, you can also call forceRenewalOfSubscription(productIdentifier:) to prompt a subscription to renew immediately.

The time rate also affects the length of the billing retry period and the billing grace period in the test environment. See the SKTestSession.TimeRate enumeration for the actual time values of each case.

Changing this property overrides its setting in the StoreKit configuration file for this test session. Call resetToDefaultState() to revert all settings to those in the configuration file.

## See Also

### Testing subscription renewals

enum TimeRate

The values for rates of time passing in the test environment.

func enableAutoRenewForTransaction(identifier: Int) throws

Enables auto-renewing for an auto-renewable subscription in the test environment.

func disableAutoRenewForTransaction(identifier: Int) throws

Disables auto-renewing for an auto-renewable subscription in the test environment.

func forceRenewalOfSubscription(productIdentifier: String) throws

Ends the previous subscription period and begins the next period in the test environment.

func expireSubscription(productIdentifier: String) throws

Causes the identified auto-renewable subscription to expire immediately in the test environment.

