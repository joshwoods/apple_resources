

- Foundation
- Date
- Date.FormatStyle
-  locale 

Instance Property

# locale

The locale to use when formatting the date and time components.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var locale: Locale
```

## Discussion

The default value is autoupdatingCurrent. If you set this property to `nil`, the formatter resets to using `autoupdatingCurrent.`

## See Also

### Modifying a Date Format Style

var timeZone: TimeZone

The time zone to use when formatting the date and time components.

var calendar: Calendar

The calendar to use when formatting the date.

var capitalizationContext: FormatStyleCapitalizationContext

The capitalization context to use when formatting the date.

