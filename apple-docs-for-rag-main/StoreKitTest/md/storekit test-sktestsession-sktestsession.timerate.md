

- StoreKit Test
- SKTestSession
-  SKTestSession.TimeRate 

Enumeration

# SKTestSession.TimeRate

The values for rates of time passing in the test environment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
enum TimeRate
```

## Overview

The time rates that affect subscription renewals in the test environment match those in the sandbox environment with these exceptions:

- Only the test environment supports the SKTestSession.TimeRate.monthlyRenewalEveryThirtySeconds time rate.

- Only the test environment supports the fixed time rate options: SKTestSession.TimeRate.oneRenewalEveryFifteenMinutes, SKTestSession.TimeRate.oneRenewalEveryFiveMinutes, SKTestSession.TimeRate.oneRenewalEveryMinute, SKTestSession.TimeRate.oneRenewalEveryThirtySeconds, SKTestSession.TimeRate.oneRenewalEveryTenSeconds, and SKTestSession.TimeRate.oneRenewalEveryTwoSeconds.

- Only the sandbox environment supports a monthly renewal in 3 minutes.

For more information about time rates in the sandbox environment, see Test in-app purchases.

The time rates also affect the lengths of the billing retry period and the billing grace period in the testing environment. See the individual enumeration cases for the actual time values of the subscription renewal rates, billing retry periods, and billing grace periods.

## Topics

### Fixed time rates for subscription renewals

case oneRenewalEveryFifteenMinutes

A rate of time in the test environment in which subscriptions of any time length renew every 15 minutes.

case oneRenewalEveryFiveMinutes

A rate of time in the test environment in which subscriptions of any time length renew every 5 minutes.

case oneRenewalEveryMinute

A rate of time in the test environment in which subscriptions of any time length renew every minute.

case oneRenewalEveryThirtySeconds

A rate of time in the test environment in which subscriptions of any time length renew every 30 seconds.

case oneRenewalEveryTenSeconds

A rate of time in the test environment in which subscriptions of any time length renew every 10 seconds.

case oneRenewalEveryTwoSeconds

A rate of time in the test environment in which subscriptions of any time length renew every 2 seconds.

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

case monthlyRenewalEveryThirtySeconds

A rate of time in the test environment in which monthly subscriptions renew every 30 seconds.

### Deprecated

case oneHourIsOneDay

A rate of time in which 1 hour in the test environment represents one day.

Deprecated

case thirtyMinutesIsOneDay

A rate of time in which 30 minutes in the test environment represents one day.

Deprecated

case fiveMinutesIsOneDay

A rate of time in which 5 minutes in the test environment represents one day.

Deprecated

case oneMinuteIsOneDay

A rate of time in which 1 minute in the test environment represents one day.

Deprecated

case thirtySecondsIsOneDay

A rate of time in which 30 seconds in the test environment represents one day.

Deprecated

case oneSecondIsOneDay

A rate of time in which 1 second in the test environment represents one day.

Deprecated

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Testing subscription renewals

var timeRate: SKTestSession.TimeRate

The rate at which time passes for subscriptions in the test environment as compared to real time.

func enableAutoRenewForTransaction(identifier: Int) throws

Enables auto-renewing for an auto-renewable subscription in the test environment.

func disableAutoRenewForTransaction(identifier: Int) throws

Disables auto-renewing for an auto-renewable subscription in the test environment.

func forceRenewalOfSubscription(productIdentifier: String) throws

Ends the previous subscription period and begins the next period in the test environment.

func expireSubscription(productIdentifier: String) throws

Causes the identified auto-renewable subscription to expire immediately in the test environment.

