

- StoreKit Test
- SKTestSession
- SKTestSession.TimeRate
-  SKTestSession.TimeRate.monthlyRenewalEveryThirtyMinutes 

Case

# SKTestSession.TimeRate.monthlyRenewalEveryThirtyMinutes

A rate of time in the test environment in which monthly subscriptions renew every 30 minutes.

iOS 15.2+iPadOS 15.2+Mac Catalyst 15.2+macOS 12.1+tvOS 15.2+visionOS 1.0+watchOS 8.3+

``` source
case monthlyRenewalEveryThirtyMinutes
```

## Discussion

The following table shows how this time rate affects subscriptions with various renewal periods in the testing environment:

| Subscription renewal period | Renewal time      |
|-----------------------------|-------------------|
| Weekly                      | 10 minutes        |
| Monthly                     | 30 minutes        |
| Bimonthly                   | 1 hour            |
| Quarterly                   | 1 hour 30 minutes |
| Semiannually                | 3 hours           |
| Annually                    | 6 hours           |

The sandbox environment also supports this subscription renewal rate. For more information about renewal rates in the sandbox environment, see Test in-app purchases.

The time rate also affects the billing grace period and the billing retry period in the testing environment, as the table below shows:

| Type | Time period |
|----|----|
| Grace period for subscriptions with a weekly renewal period | 8 minutes 34 seconds |
| Grace period for subscriptions with all other renewal periods | 15 minutes |
| Billing retry period | 1 hour |

## See Also

### Scaled time rates for subscription renewals

case realTime

A rate of time in which the test environment runs in real time.

case monthlyRenewalEveryHour

A rate of time in the test environment in which monthly subscriptions renew every hour.

case monthlyRenewalEveryFifteenMinutes

A rate of time in the test environment in which monthly subscriptions renew every 15 minutes.

case monthlyRenewalEveryFiveMinutes

A rate of time in the test environment in which monthly subscriptions renew every 5 minutes.

case monthlyRenewalEveryThirtySeconds

A rate of time in the test environment in which monthly subscriptions renew every 30 seconds.

