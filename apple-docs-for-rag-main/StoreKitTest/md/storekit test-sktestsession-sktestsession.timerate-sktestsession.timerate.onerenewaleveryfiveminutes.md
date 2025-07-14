

- StoreKit Test
- SKTestSession
- SKTestSession.TimeRate
-  SKTestSession.TimeRate.oneRenewalEveryFiveMinutes 

Case

# SKTestSession.TimeRate.oneRenewalEveryFiveMinutes

A rate of time in the test environment in which subscriptions of any time length renew every 5 minutes.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
case oneRenewalEveryFiveMinutes
```

## Discussion

This time rate renews subscriptions every five minutes in the testing environment, regardless of actual renewal periods for each subscription.

The sandbox environment does not support this subscription renewal rate.

This time rate also affects the billing grace period and the billing retry period in the testing environment, as the table below shows:

| Type                                                    | Time Period |
|---------------------------------------------------------|-------------|
| Grace period for subscriptions with all renewal periods | 5 minutes   |
| Billing retry period                                    | 10 minutes  |

## See Also

### Fixed time rates for subscription renewals

case oneRenewalEveryFifteenMinutes

A rate of time in the test environment in which subscriptions of any time length renew every 15 minutes.

case oneRenewalEveryMinute

A rate of time in the test environment in which subscriptions of any time length renew every minute.

case oneRenewalEveryThirtySeconds

A rate of time in the test environment in which subscriptions of any time length renew every 30 seconds.

case oneRenewalEveryTenSeconds

A rate of time in the test environment in which subscriptions of any time length renew every 10 seconds.

case oneRenewalEveryTwoSeconds

A rate of time in the test environment in which subscriptions of any time length renew every 2 seconds.

