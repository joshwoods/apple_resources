

- ClockKit
- CLKTimeIntervalTextProvider
-  startDate Deprecated

Instance Property

# startDate

The start date for the time interval.

watchOS 2.0–9.0Deprecated

``` source
var startDate: Date { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

The date in this property must come chronologically before the date in the endDate property. This property must not be `nil`.

## See Also

### Related Documentation

convenience init(start: Date, end: Date, timeZone: TimeZone?)

Creates and returns a text provider with the specified dates and time zone information.

Deprecated

convenience init(start: Date, end: Date)

Creates and returns a text provider with the specified start and end dates.

Deprecated

### Getting the Time Information

var endDate: Date

The end date for the time interval.

Deprecated

var timeZone: TimeZone?

The time zone used to format time values.

Deprecated

