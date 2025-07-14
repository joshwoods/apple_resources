

- Foundation
- DateIntervalFormatter
-  dateTemplate 

Instance Property

# dateTemplate

The template for formatting one date and time value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var dateTemplate: String! { get set }
```

## Discussion

Use this string to specify a custom fixed format for each of the date and time values. The string you specify is based on the Unicode Technical Standard \#35, which uses characters to represent the day, time, year, hour, minute, and other pieces of date or time information.

If you do not assign a value to this string, the formatter object automatically updates the string based on the values in the dateStyle and timeStyle properties.

For information about how to define a custom formatting string, see Date Formatters in Data Formatting Guide.

## See Also

### Configuring the Formatter Options

var dateStyle: DateIntervalFormatter.Style

The style to use when formatting day, month, and year information.

var timeStyle: DateIntervalFormatter.Style

The style to use when formatting hour, minute, and second information.

var calendar: Calendar!

The calendar to use for date values.

var locale: Locale!

The locale to use when formatting date and time values.

var timeZone: TimeZone!

The time zone with which to specify time values.

