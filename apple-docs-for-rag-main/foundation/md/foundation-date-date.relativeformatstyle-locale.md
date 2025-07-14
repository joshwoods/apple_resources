

- Foundation
- Date
- Date.RelativeFormatStyle
-  locale 

Instance Property

# locale

The locale to use when formatting the relative date.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var locale: Locale
```

## Discussion

The default value is autoupdatingCurrent. If you set this property to `nil`, the format style resets to using autoupdatingCurrent.

## See Also

### Modifying a Relative Date Format Style

var presentation: Date.RelativeFormatStyle.Presentation

Specifies the style to use when describing a relative date, such as “1 day ago” or “yesterday”.

var unitsStyle: Date.RelativeFormatStyle.UnitsStyle

The style to use when formatting the quantity or the name of the unit, such as “1 day ago” or “one day ago”.

var calendar: Calendar

The calendar to use when formatting relative dates.

var capitalizationContext: FormatStyleCapitalizationContext

The capitalization context to use when formatting the relative dates.

