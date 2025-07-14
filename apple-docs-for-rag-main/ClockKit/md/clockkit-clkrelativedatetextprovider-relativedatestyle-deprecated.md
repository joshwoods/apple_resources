

- ClockKit
- CLKRelativeDateTextProvider
-  relativeDateStyle Deprecated

Instance Property

# relativeDateStyle

The formatting style to use for the relative time value.

watchOS 2.0–9.0Deprecated

``` source
var relativeDateStyle: CLKRelativeDateStyle { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

For a list of possible values, see CLKRelativeDateStyle.

## See Also

### Getting the Date Information

var date: Date

The target date to use for calculations.

Deprecated

var relativeToDate: Date?

The end date that the text provider uses when calculating a fixed, relative date.

Deprecated

var calendarUnits: NSCalendar.Unit

The calendar units to include in the formatted string.

Deprecated

