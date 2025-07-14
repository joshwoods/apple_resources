

- StoreKit
- Product
- Product.SubscriptionPeriod
-  formatted(\_:referenceDate:) 

Instance Method

# formatted(\_:referenceDate:)

Formats the subscription period using a format style that takes a date range as an input.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@backDeployed(before: iOS 16.0, macOS 13.0, tvOS 16.0, watchOS 9.0, macCatalyst 16.0)
func formatted(
    _ format: S,
    referenceDate: Date = .now
) -> S.FormatOutput where S : FormatStyle, S.FormatInput == Range
```

## Parameters 

`format`  

A format style that has a date range input. The format style for a product is subscriptionPeriodFormatStyle.

`referenceDate`  

The lower bound date for a date range representing the subscription period. The default value is now.

## Discussion

Use the formatted(_:referenceDate:) method with subscriptionPeriodFormatStyle to format the subscription period for the App Store locale, as the following example shows.

```
// Get a human-readable representation of a subscription period.
subscriptionPeriod.formatted(product.subscriptionPeriodFormatStyle, referenceDate: /* some date */)

```

## See Also

### Formatting the subscription period

func formatted&lt;S>(S, referenceDate: Date) -> S.FormatOutput

Formats the subscription period using a format style that takes a duration as an input.

