

- StoreKit Test
- SKTestSession
- SKTestSession.TimeRate
-  SKTestSession.TimeRate.monthlyRenewalEveryFifteenMinutes 

Case

# SKTestSession.TimeRate.monthlyRenewalEveryFifteenMinutes

A rate of time in the test environment in which monthly subscriptions renew every 15 minutes.

iOS 15.2+iPadOS 15.2+Mac Catalyst 15.2+macOS 12.1+tvOS 15.2+visionOS 1.0+watchOS 8.3+

``` source
case monthlyRenewalEveryFifteenMinutes
```

## Discussion

The following table shows how this time rate affects subscriptions with various renewal periods in the testing environment:

| Subscription renewal period | Renewal time      |
|-----------------------------|-------------------|
| Weekly                      | 5 minutes         |
| Monthly                     | 15 minutes        |
| Bimonthly                   | 30 minutes        |
| Quarterly                   | 45 minutes        |
| Semiannually                | 1 hour 30 minutes |
| Annually                    | 3 hours           |

The sandbox environment also supports this subscription renewal rate. For more information about renewal rates in the sandbox environment, see Test in-app purchases.

The time rate also affects the billing grace period and the billing retry period in the testing environment, as the table below shows:

| Type | Time period |
|----|----|
| Grace period for subscriptions with a weekly renewal period | 4 minutes 17 seconds |
| Grace period for subscriptions with all other renewal periods | 7 minutes 30 seconds |
| Billing retry period | 30 minutes |

## See Also

### Scaled time rates for subscription renewals

case realTime

A rate of time in which the test environment runs in real time.

case monthlyRenewalEveryHour

A rate of time in the test environment in which monthly subscriptions renew every hour.

case monthlyRenewalEveryThirtyMinutes

A rate of time in the test environment in which monthly subscriptions renew every 30 minutes.

case monthlyRenewalEveryFiveMinutes

A rate of time in the test environment in which monthly subscriptions renew every 5 minutes.

case monthlyRenewalEveryThirtySeconds

A rate of time in the test environment in which monthly subscriptions renew every 30 seconds.

