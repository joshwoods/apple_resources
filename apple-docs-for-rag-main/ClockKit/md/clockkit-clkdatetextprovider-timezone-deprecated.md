

- ClockKit
- CLKDateTextProvider
-  timeZone Deprecated

Instance Property

# timeZone

The time zone used in the formatted string.

watchOS 2.0–9.0Deprecated

``` source
var timeZone: TimeZone? { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

The date provider uses the time zone information during formatting to ensure that the date information is displayed correctly. To use the current time zone, set this property to `nil`.

## See Also

### Getting the Date Information

var date: Date

The date to display.

Deprecated

var calendarUnits: NSCalendar.Unit

The calendar units to include in the formatted string.

Deprecated

var uppercase: Bool

A Boolean value that determines whether the date string displays in uppercase.

Deprecated

