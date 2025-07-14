

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.TimeStyle
-  shortened 

Type Property

# shortened

A shortened time style with only the hour, minute, and day period components represented.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let shortened: Date.FormatStyle.TimeStyle
```

## Discussion

A `shortened` time style represents the hour, minute, and day period components in the format. For example, `9:54 PM.`

## See Also

### Modifying a Time Style

static let complete: Date.FormatStyle.TimeStyle

A time style with all components represented.

static let omitted: Date.FormatStyle.TimeStyle

A time style with no time-related components represented.

static let standard: Date.FormatStyle.TimeStyle

A time style with all components except the time zone represented.

