

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.DateStyle
-  long 

Type Property

# long

A lengthened date style with the full month, day of month, and year components represented.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let long: Date.FormatStyle.DateStyle
```

## Discussion

A `long` date style represents the full date without the day of week in the format. For example, `October 17, 2020`.

## See Also

### Modifying a Date Style

static let abbreviated: Date.FormatStyle.DateStyle

A date style with some components abbreviated for space-constrained applications.

static let complete: Date.FormatStyle.DateStyle

A date style with all components represented.

static let numeric: Date.FormatStyle.DateStyle

A date style with the month, day of month, and year components represented as numeric values.

static let omitted: Date.FormatStyle.DateStyle

A date style with no date-related components represented.

