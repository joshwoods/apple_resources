

- StoreKit
- SKProductSubscriptionPeriod
-  numberOfUnits Deprecated

Instance Property

# numberOfUnits

The number of units per subscription period.

iOS 11.2–18.0DeprecatediPadOS 11.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13.2–15.0DeprecatedtvOS 11.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var numberOfUnits: Int { get }
```

Deprecated

Use Product.SubscriptionPeriod

## Discussion

A subscription period duration is calculated by multiplying the number of units by the unit.

For example, if the number of units is `3`, and the unit is SKProduct.PeriodUnit.month, the subscription period is 3 months.

## See Also

### Getting Subscription Period Details

var unit: SKProduct.PeriodUnit

The increment of time that a subscription period is specified in.

Deprecated

enum PeriodUnit

Values representing the duration of an interval, from a day up to a year.

Deprecated

