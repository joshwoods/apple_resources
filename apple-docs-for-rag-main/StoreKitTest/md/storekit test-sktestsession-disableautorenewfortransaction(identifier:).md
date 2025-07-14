

- StoreKit Test
- SKTestSession
-  disableAutoRenewForTransaction(identifier:) 

Instance Method

# disableAutoRenewForTransaction(identifier:)

Disables auto-renewing for an auto-renewable subscription in the test environment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func disableAutoRenewForTransaction(identifier: Int) throws
```

## Parameters 

`identifier`  

The transaction identifier of the auto-renewable subscription.

## Discussion

Call this method to disable auto-renewing for a subscription. A subscription with auto-renew disabled expires at the end of the billing period and doesn’t renew at the start of the next billing period.

## See Also

### Testing subscription renewals

var timeRate: SKTestSession.TimeRate

The rate at which time passes for subscriptions in the test environment as compared to real time.

enum TimeRate

The values for rates of time passing in the test environment.

func enableAutoRenewForTransaction(identifier: Int) throws

Enables auto-renewing for an auto-renewable subscription in the test environment.

func forceRenewalOfSubscription(productIdentifier: String) throws

Ends the previous subscription period and begins the next period in the test environment.

func expireSubscription(productIdentifier: String) throws

Causes the identified auto-renewable subscription to expire immediately in the test environment.

