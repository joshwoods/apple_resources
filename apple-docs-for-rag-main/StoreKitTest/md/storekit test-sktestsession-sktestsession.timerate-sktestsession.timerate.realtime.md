

- StoreKit Test
- SKTestSession
- SKTestSession.TimeRate
-  SKTestSession.TimeRate.realTime 

Case

# SKTestSession.TimeRate.realTime

A rate of time in which the test environment runs in real time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
case realTime
```

## Discussion

With this time rate, subscriptions in the testing environment renew in real time. For example, a weekly subscription renews in one week.

The time rate also affects the billing grace period and the billing retry period in the testing environment. The table below shows the real-time rates:

| Type                                                          | Time period |
|---------------------------------------------------------------|-------------|
| Grace period for subscriptions with a weekly renewal period   | 6 days      |
| Grace period for subscriptions with all other renewal periods | 16 days     |
| Billing retry period                                          | 60 days     |

## See Also

### Scaled time rates for subscription renewals

case monthlyRenewalEveryHour

A rate of time in the test environment in which monthly subscriptions renew every hour.

case monthlyRenewalEveryThirtyMinutes

A rate of time in the test environment in which monthly subscriptions renew every 30 minutes.

case monthlyRenewalEveryFifteenMinutes

A rate of time in the test environment in which monthly subscriptions renew every 15 minutes.

case monthlyRenewalEveryFiveMinutes

A rate of time in the test environment in which monthly subscriptions renew every 5 minutes.

case monthlyRenewalEveryThirtySeconds

A rate of time in the test environment in which monthly subscriptions renew every 30 seconds.

