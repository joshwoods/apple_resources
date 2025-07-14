

- Foundation
- Date
- Date.FormatStyle
- 
  - Date
  - Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.Hour
- Date.FormatStyle.Symbol.Hour.AMPMStyle
-  abbreviated 

Type Property

# abbreviated

A type that specifies the abbreviated day period for when the locale prefers using day period with hour.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let abbreviated: Date.FormatStyle.Symbol.Hour.AMPMStyle
```

## Discussion

This type represents the hour period in an abbreviated format where appropriate. For example, when used with `defaultDigits`, this style may represent 8 a.m. as `8`, or `8 AM`, and 1 p.m. as `13`, or `1 PM`. With `twoDigits`, this style produces `08` or `08 AM`, and `13`, `01 PM`, respectively.

## See Also

### Creating AMPM Styles

static let narrow: Date.FormatStyle.Symbol.Hour.AMPMStyle

A type that specifies the narrow day period if the locale prefers using day period with hour.

static let omitted: Date.FormatStyle.Symbol.Hour.AMPMStyle

A type that hides the day period marker.

static let wide: Date.FormatStyle.Symbol.Hour.AMPMStyle

A type that represents the wide day period if the locale prefers using day period with hour.

