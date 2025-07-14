

- StoreKit
-  SKProductSubscriptionPeriod Deprecated

Class

# SKProductSubscriptionPeriod

An object containing the subscription period duration information.

iOS 11.2–18.0DeprecatediPadOS 11.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13.2–15.0DeprecatedtvOS 11.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class SKProductSubscriptionPeriod
```

Deprecated

Use Product.SubscriptionPeriod

## Overview

A subscription period is a duration of time defined as some number of units, where a unit can be a SKProduct.PeriodUnit.day, SKProduct.PeriodUnit.week, SKProduct.PeriodUnit.month, or SKProduct.PeriodUnit.year.

For example, a subscription period of two weeks has a unit of a SKProduct.PeriodUnit.week, and a numberOfUnits equal to `2`.

## Topics

### Getting Subscription Period Details

var numberOfUnits: Int

The number of units per subscription period.

var unit: SKProduct.PeriodUnit

The increment of time that a subscription period is specified in.

enum PeriodUnit

Values representing the duration of an interval, from a day up to a year.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Getting Subscription Information

var subscriptionGroupIdentifier: String?

The identifier of the subscription group to which the subscription belongs.

Deprecated

var subscriptionPeriod: SKProductSubscriptionPeriod?

The period details for products that are subscriptions.

Deprecated

enum PeriodUnit

Values representing the duration of an interval, from a day up to a year.

Deprecated

