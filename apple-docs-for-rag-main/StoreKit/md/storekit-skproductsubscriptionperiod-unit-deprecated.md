

- StoreKit
- SKProductSubscriptionPeriod
-  unit Deprecated

Instance Property

# unit

The increment of time that a subscription period is specified in.

iOS 11.2–18.0DeprecatediPadOS 11.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13.2–15.0DeprecatedtvOS 11.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var unit: SKProduct.PeriodUnit { get }
```

Deprecated

Use Product.SubscriptionPeriod

## Discussion

The units used to specify a subscription period include day, week, month, and year, as defined in SKProduct.PeriodUnit.

To calculate the duration of one subscription period, multiply the unit by the number of units (numberOfUnits).

## See Also

### Getting Subscription Period Details

var numberOfUnits: Int

The number of units per subscription period.

Deprecated

enum PeriodUnit

Values representing the duration of an interval, from a day up to a year.

Deprecated

