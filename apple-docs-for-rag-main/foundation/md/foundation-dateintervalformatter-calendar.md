

- Foundation
- DateIntervalFormatter
-  calendar 

Instance Property

# calendar

The calendar to use for date values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var calendar: Calendar! { get set }
```

## Discussion

The default value of this property is the calendar associated with the current locale object. You can change this value to use a different calendar for interpreting dates.

## See Also

### Configuring the Formatter Options

var dateStyle: DateIntervalFormatter.Style

The style to use when formatting day, month, and year information.

var timeStyle: DateIntervalFormatter.Style

The style to use when formatting hour, minute, and second information.

var dateTemplate: String!

The template for formatting one date and time value.

var locale: Locale!

The locale to use when formatting date and time values.

var timeZone: TimeZone!

The time zone with which to specify time values.

