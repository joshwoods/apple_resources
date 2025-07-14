

- ClockKit
- CLKTimeIntervalTextProvider
-  timeZone Deprecated

Instance Property

# timeZone

The time zone used to format time values.

watchOS 2.0–9.0Deprecated

``` source
var timeZone: TimeZone? { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

If the value is `nil`, the text provider uses the time zone currently configured for the user.

## See Also

### Related Documentation

convenience init(start: Date, end: Date, timeZone: TimeZone?)

Creates and returns a text provider with the specified dates and time zone information.

Deprecated

### Getting the Time Information

var startDate: Date

The start date for the time interval.

Deprecated

var endDate: Date

The end date for the time interval.

Deprecated

