

- StoreKit Test
- SKTestSession
-  forceRenewalOfSubscription(productIdentifier:) 

Instance Method

# forceRenewalOfSubscription(productIdentifier:)

Ends the previous subscription period and begins the next period in the test environment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func forceRenewalOfSubscription(productIdentifier: String) throws
```

## Parameters 

`productIdentifier`  

The productIdentifier of the auto-renewable subscription to renew.

## Discussion

Use this method to test how your code handles subscription renewals. When you call this method, the subscription expires at the time you call the method, and a new subscription period begins.

To force the subscription renewal, the testing environment changes the expirationDate property on the Transaction to the current system time. (If your app uses receipts, the receipt also shows this expiration date change). The testing environment also:

- Enables the subscription auto-renew state

- Removes a pending price increase, setting it to Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus.noIncreasePending

The testing environment doesn’t change the billing retry state with this call.

You can also test subscription renewals by accelerating the time in the testing environment to speed up subscription renewal periods. See timeRate for more information.

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

func expireSubscription(productIdentifier: String) throws

Causes the identified auto-renewable subscription to expire immediately in the test environment.

