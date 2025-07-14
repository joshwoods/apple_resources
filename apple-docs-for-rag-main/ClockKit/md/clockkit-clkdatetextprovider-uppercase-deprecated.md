

- ClockKit
- CLKDateTextProvider
-  uppercase Deprecated

Instance Property

# uppercase

A Boolean value that determines whether the date string displays in uppercase.

watchOS 2.0–9.0Deprecated

``` source
var uppercase: Bool { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

By default, this property is set to false. Set it to true if you want the text provider to produce uppercase text.

## See Also

### Getting the Date Information

var date: Date

The date to display.

Deprecated

var timeZone: TimeZone?

The time zone used in the formatted string.

Deprecated

var calendarUnits: NSCalendar.Unit

The calendar units to include in the formatted string.

Deprecated

