

- StoreKit
- Product
- Product.SubscriptionPeriod
-  Product.SubscriptionPeriod.Unit 

Enumeration

# Product.SubscriptionPeriod.Unit

Units of time that describe subscription periods.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Unit
```

## Topics

### Getting the subscription period units

case day

A subscription period unit of a day.

case month

A subscription period unit of a month.

case week

A subscription period unit of a week.

case year

A subscription period unit of a year.

### Getting localized and debug descriptions

var localizedDescription: String

The localized text that describes the subscription period unit.

### Getting the formatted description

func formatted&lt;S>(S) -> S.FormatOutput

struct FormatStyle

## Relationships

### Conforms To

- Comparable
- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Getting the subscription period

let value: Int

The number of period units.

let unit: Product.SubscriptionPeriod.Unit

The increment of time for the subscription period.

