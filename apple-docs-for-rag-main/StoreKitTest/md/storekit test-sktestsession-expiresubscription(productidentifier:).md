

- StoreKit Test
- SKTestSession
-  expireSubscription(productIdentifier:) 

Instance Method

# expireSubscription(productIdentifier:)

Causes the identified auto-renewable subscription to expire immediately in the test environment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func expireSubscription(productIdentifier: String) throws
```

## Parameters 

`productIdentifier`  

The productIdentifier of the auto-renewable subscription to expire.

## Discussion

Use this method to test how your app handles expired subscriptions and revoking access to content or service. This method forces the subscription to expire. Specifically, the testing environment disables auto-renew and changes the subscription’s expiration date to the current system time.

You can also test subscription expiration by accelerating the time in the testing environment to speed up subscription renewal periods. See timeRate for more information.

## See Also

### Testing subscription renewals

var timeRate: SKTestSession.TimeRate

The rate at which time passes for subscriptions in the test environment as compared to real time.

enum TimeRate

The values for rates of time passing in the test environment.

func enableAutoRenewForTransaction(identifier: Int) throws

Enables auto-renewing for an auto-renewable subscription in the test environment.

func disableAutoRenewForTransaction(identifier: Int) throws

Disables auto-renewing for an auto-renewable subscription in the test environment.

func forceRenewalOfSubscription(productIdentifier: String) throws

Ends the previous subscription period and begins the next period in the test environment.

