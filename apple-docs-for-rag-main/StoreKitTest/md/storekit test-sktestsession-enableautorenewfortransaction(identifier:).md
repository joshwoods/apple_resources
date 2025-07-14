

- StoreKit Test
- SKTestSession
-  enableAutoRenewForTransaction(identifier:) 

Instance Method

# enableAutoRenewForTransaction(identifier:)

Enables auto-renewing for an auto-renewable subscription in the test environment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func enableAutoRenewForTransaction(identifier: Int) throws
```

## Parameters 

`identifier`  

The transaction identifier of the auto-renewable subscription.

## Discussion

Call this method to enable the subscription to automatically renew in the testing environment. By default, all auto-renewable subscriptions have auto-renew enabled.

## See Also

### Testing subscription renewals

var timeRate: SKTestSession.TimeRate

The rate at which time passes for subscriptions in the test environment as compared to real time.

enum TimeRate

The values for rates of time passing in the test environment.

func disableAutoRenewForTransaction(identifier: Int) throws

Disables auto-renewing for an auto-renewable subscription in the test environment.

func forceRenewalOfSubscription(productIdentifier: String) throws

Ends the previous subscription period and begins the next period in the test environment.

func expireSubscription(productIdentifier: String) throws

Causes the identified auto-renewable subscription to expire immediately in the test environment.

