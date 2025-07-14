

- Foundation
- Date
- Date.FormatStyle
- 
  - Date
  - Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.Hour
- Date.FormatStyle.Symbol.Hour.AMPMStyle
-  omitted 

Type Property

# omitted

A type that hides the day period marker.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let omitted: Date.FormatStyle.Symbol.Hour.AMPMStyle
```

## Discussion

This type represents the hour period numerically only. For example, `8` (for 8 a.m.) or `1` (for 1 p.m.) if used with `defaultDigits`, and `08` or `01` if used with `twoDigits`.

## See Also

### Creating AMPM Styles

static let abbreviated: Date.FormatStyle.Symbol.Hour.AMPMStyle

A type that specifies the abbreviated day period for when the locale prefers using day period with hour.

static let narrow: Date.FormatStyle.Symbol.Hour.AMPMStyle

A type that specifies the narrow day period if the locale prefers using day period with hour.

static let wide: Date.FormatStyle.Symbol.Hour.AMPMStyle

A type that represents the wide day period if the locale prefers using day period with hour.

