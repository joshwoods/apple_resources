

- StoreKit
- SKProductDiscount
-  subscriptionPeriod Deprecated

Instance Property

# subscriptionPeriod

An object that defines the period for the product discount.

iOS 11.2–18.0DeprecatediPadOS 11.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13.2–15.0DeprecatedtvOS 11.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var subscriptionPeriod: SKProductSubscriptionPeriod { get }
```

Deprecated

Use Product.SubscriptionOffer.period

## Discussion

This object represents the duration of a single subscription period. A period is described as a number of units, where a unit can be a SKProduct.PeriodUnit.day, SKProduct.PeriodUnit.month, SKProduct.PeriodUnit.week, or SKProduct.PeriodUnit.year.

To calculate the total amount of time that the discount price is available to the user, multiply the subscriptionPeriod by numberOfPeriods.

Note

The subscription period for the discount is independent of the product’s regular subscription period, and does not have to match in units or duration.

## See Also

### Getting the Discount Duration

var numberOfPeriods: Int

An integer that indicates the number of periods the product discount is available.

Deprecated

