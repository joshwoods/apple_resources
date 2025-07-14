

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.TimeStyle
-  omitted 

Type Property

# omitted

A time style with no time-related components represented.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let omitted: Date.FormatStyle.TimeStyle
```

## Discussion

If both the date style and time style are set to `omitted`, the time is represented using the default style of `shortened`.

## See Also

### Modifying a Time Style

static let complete: Date.FormatStyle.TimeStyle

A time style with all components represented.

static let shortened: Date.FormatStyle.TimeStyle

A shortened time style with only the hour, minute, and day period components represented.

static let standard: Date.FormatStyle.TimeStyle

A time style with all components except the time zone represented.

