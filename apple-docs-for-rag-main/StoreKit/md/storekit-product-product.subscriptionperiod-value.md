

- StoreKit
- Product
- Product.SubscriptionPeriod
-  value 

Instance Property

# value

The number of period units.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let value: Int
```

## Discussion

Use the value and the unit together to determine the subscription period. For example, if the unit is Product.SubscriptionPeriod.Unit.month, and the value is `3`, the subscription period is three months.

## See Also

### Getting the subscription period

let unit: Product.SubscriptionPeriod.Unit

The increment of time for the subscription period.

enum Unit

Units of time that describe subscription periods.

