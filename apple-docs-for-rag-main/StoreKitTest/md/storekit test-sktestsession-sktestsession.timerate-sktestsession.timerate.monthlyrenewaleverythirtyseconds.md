

- StoreKit Test
- SKTestSession
- SKTestSession.TimeRate
-  SKTestSession.TimeRate.monthlyRenewalEveryThirtySeconds 

Case

# SKTestSession.TimeRate.monthlyRenewalEveryThirtySeconds

A rate of time in the test environment in which monthly subscriptions renew every 30 seconds.

iOS 15.2+iPadOS 15.2+Mac Catalyst 15.2+macOS 12.1+tvOS 15.2+visionOS 1.0+watchOS 8.3+

``` source
case monthlyRenewalEveryThirtySeconds
```

## Discussion

The following table shows how this time rate affects subscriptions with various renewal periods in the testing environment:

| Subscription renewal period | Renewal time        |
|-----------------------------|---------------------|
| Weekly                      | 10 seconds          |
| Monthly                     | 30 seconds          |
| Bimonthly                   | 1 minute            |
| Quarterly                   | 1 minute 30 seconds |
| Semiannually                | 3 minutes           |
| Annually                    | 6 minutes           |

The sandbox environment doesn’t have an equivalent subscription renewal rate for SKTestSession.TimeRate.monthlyRenewalEveryThirtySeconds. For more information about renewal rates in the sandbox environment, see Test in-app purchases.

The time rate also affects the billing grace period and the billing retry period in the testing environment, as the table below shows:

| Type                                                          | Time period |
|---------------------------------------------------------------|-------------|
| Grace period for subscriptions with a weekly renewal period   | 9 seconds   |
| Grace period for subscriptions with all other renewal periods | 15 seconds  |
| Billing retry period                                          | 1 minute    |

## See Also

### Scaled time rates for subscription renewals

case realTime

A rate of time in which the test environment runs in real time.

case monthlyRenewalEveryHour

A rate of time in the test environment in which monthly subscriptions renew every hour.

case monthlyRenewalEveryThirtyMinutes

A rate of time in the test environment in which monthly subscriptions renew every 30 minutes.

case monthlyRenewalEveryFifteenMinutes

A rate of time in the test environment in which monthly subscriptions renew every 15 minutes.

case monthlyRenewalEveryFiveMinutes

A rate of time in the test environment in which monthly subscriptions renew every 5 minutes.

