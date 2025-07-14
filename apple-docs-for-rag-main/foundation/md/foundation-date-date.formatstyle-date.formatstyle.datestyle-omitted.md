

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.DateStyle
-  omitted 

Type Property

# omitted

A date style with no date-related components represented.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let omitted: Date.FormatStyle.DateStyle
```

## Discussion

If both the date style and time style are set to `omitted`, the date is represented using the default style of `abbreviated`.

## See Also

### Modifying a Date Style

static let abbreviated: Date.FormatStyle.DateStyle

A date style with some components abbreviated for space-constrained applications.

static let complete: Date.FormatStyle.DateStyle

A date style with all components represented.

static let long: Date.FormatStyle.DateStyle

A lengthened date style with the full month, day of month, and year components represented.

static let numeric: Date.FormatStyle.DateStyle

A date style with the month, day of month, and year components represented as numeric values.

