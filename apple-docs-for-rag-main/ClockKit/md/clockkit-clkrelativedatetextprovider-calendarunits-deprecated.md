

- ClockKit
- CLKRelativeDateTextProvider
-  calendarUnits Deprecated

Instance Property

# calendarUnits

The calendar units to include in the formatted string.

watchOS 2.0–9.0Deprecated

``` source
var calendarUnits: NSCalendar.Unit { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

For a list of supported units, see Date Format Options.

## See Also

### Getting the Date Information

var date: Date

The target date to use for calculations.

Deprecated

var relativeToDate: Date?

The end date that the text provider uses when calculating a fixed, relative date.

Deprecated

var relativeDateStyle: CLKRelativeDateStyle

The formatting style to use for the relative time value.

Deprecated

