

- StoreKit
- Product
- Product.SubscriptionPeriod
-  formatted(\_:referenceDate:) 

Instance Method

# formatted(\_:referenceDate:)

Formats the subscription period using a format style that takes a duration as an input.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func formatted(
    _ format: S,
    referenceDate: Date = .now
) -> S.FormatOutput where S : FormatStyle, S.FormatInput == Duration
```

## Parameters 

`format`  

A format style that has a duration as an input.

`referenceDate`  

The starting date of the subscription period. The default value is now.

## See Also

### Formatting the subscription period

func formatted&lt;S>(S, referenceDate: Date) -> S.FormatOutput

Formats the subscription period using a format style that takes a date range as an input.

