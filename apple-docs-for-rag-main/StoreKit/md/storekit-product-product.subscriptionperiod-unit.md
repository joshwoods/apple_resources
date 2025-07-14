

- StoreKit
- Product
- Product.SubscriptionPeriod
-  unit 

Instance Property

# unit

The increment of time for the subscription period.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let unit: Product.SubscriptionPeriod.Unit
```

## Discussion

The units used to specify a subscription period include day, week, month, and year, as defined in Product.SubscriptionPeriod.Unit.

To calculate the duration of one subscription period, multiply the unit by the number of units (value).

## See Also

### Getting the subscription period

let value: Int

The number of period units.

enum Unit

Units of time that describe subscription periods.

