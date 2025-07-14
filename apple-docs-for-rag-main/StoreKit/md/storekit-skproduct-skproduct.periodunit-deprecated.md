

- StoreKit
- SKProduct
-  SKProduct.PeriodUnit Deprecated

Enumeration

# SKProduct.PeriodUnit

Values representing the duration of an interval, from a day up to a year.

iOS 11.2–18.0DeprecatediPadOS 11.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13.2–15.0DeprecatedtvOS 11.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
enum PeriodUnit
```

Deprecated

Use Product.SubscriptionPeriod.Unit

## Overview

The period unit represents the duration of an interval. Period units are used with the number of units to determine one period in SKProductSubscriptionPeriod.

## Topics

### Period Units

case day

An interval lasting one day.

case month

An interval lasting one month.

case week

An interval lasting one week.

case year

An interval lasting one year.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Subscription Information

var subscriptionGroupIdentifier: String?

The identifier of the subscription group to which the subscription belongs.

Deprecated

var subscriptionPeriod: SKProductSubscriptionPeriod?

The period details for products that are subscriptions.

Deprecated

class SKProductSubscriptionPeriod

An object containing the subscription period duration information.

Deprecated

