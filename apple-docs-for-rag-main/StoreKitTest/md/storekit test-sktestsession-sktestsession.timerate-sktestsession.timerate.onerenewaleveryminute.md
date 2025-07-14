

- StoreKit Test
- SKTestSession
- SKTestSession.TimeRate
-  SKTestSession.TimeRate.oneRenewalEveryMinute 

Case

# SKTestSession.TimeRate.oneRenewalEveryMinute

A rate of time in the test environment in which subscriptions of any time length renew every minute.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
case oneRenewalEveryMinute
```

## Discussion

This time rate renews subscriptions every minute in the testing environment, regardless of actual renewal periods for each subscription.

The sandbox environment does not support this subscription renewal rate.

This time rate also affects the billing grace period and the billing retry period in the testing environment, as the table below shows:

| Type                                                    | Time Period |
|---------------------------------------------------------|-------------|
| Grace period for subscriptions with all renewal periods | 1 minute    |
| Billing retry period                                    | 2 minutes   |

## See Also

### Fixed time rates for subscription renewals

case oneRenewalEveryFifteenMinutes

A rate of time in the test environment in which subscriptions of any time length renew every 15 minutes.

case oneRenewalEveryFiveMinutes

A rate of time in the test environment in which subscriptions of any time length renew every 5 minutes.

case oneRenewalEveryThirtySeconds

A rate of time in the test environment in which subscriptions of any time length renew every 30 seconds.

case oneRenewalEveryTenSeconds

A rate of time in the test environment in which subscriptions of any time length renew every 10 seconds.

case oneRenewalEveryTwoSeconds

A rate of time in the test environment in which subscriptions of any time length renew every 2 seconds.

