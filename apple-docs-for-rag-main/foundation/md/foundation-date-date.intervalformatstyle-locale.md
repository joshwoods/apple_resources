

- Foundation
- Date
- Date.IntervalFormatStyle
-  locale 

Instance Property

# locale

The locale for formatting the date and time interval components.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var locale: Locale
```

## Discussion

The default value is autoupdatingCurrent. If you set this property to `nil`, the formatter resets to use `autoupdatingCurrent.`

## See Also

### Specifying Date Interval Format Styles

func timeZone(Date.IntervalFormatStyle.Symbol.TimeZone) -> Date.IntervalFormatStyle

Modifies the date interval format style to use the specified time zone format.

var calendar: Calendar

The calendar for formatting the date interval.

var timeZone: TimeZone

The time zone for formatting the date interval components.

