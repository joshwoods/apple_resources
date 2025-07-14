

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.DateStyle
-  numeric 

Type Property

# numeric

A date style with the month, day of month, and year components represented as numeric values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let numeric: Date.FormatStyle.DateStyle
```

## Discussion

A `numeric` date style represents the date components using numeric values. For example, `10/17/2020`, for locale `en_US`.

## See Also

### Modifying a Date Style

static let abbreviated: Date.FormatStyle.DateStyle

A date style with some components abbreviated for space-constrained applications.

static let complete: Date.FormatStyle.DateStyle

A date style with all components represented.

static let long: Date.FormatStyle.DateStyle

A lengthened date style with the full month, day of month, and year components represented.

static let omitted: Date.FormatStyle.DateStyle

A date style with no date-related components represented.

