

- StoreKit
- SKProductDiscount
-  numberOfPeriods Deprecated

Instance Property

# numberOfPeriods

An integer that indicates the number of periods the product discount is available.

iOS 11.2–18.0DeprecatediPadOS 11.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13.2–15.0DeprecatedtvOS 11.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var numberOfPeriods: Int { get }
```

Deprecated

Use Product.SubscriptionOffer.periodCount

## Discussion

A product discount may be available for one or more periods. The period, defined in subscriptionPeriod, is a set number of days, weeks, months, or years.

The total length of time that a product discount is available is calculated by multiplying the numberOfPeriods by the period.

Note that the discount period is independent of the product subscription period.

## See Also

### Getting the Discount Duration

var subscriptionPeriod: SKProductSubscriptionPeriod

An object that defines the period for the product discount.

Deprecated

