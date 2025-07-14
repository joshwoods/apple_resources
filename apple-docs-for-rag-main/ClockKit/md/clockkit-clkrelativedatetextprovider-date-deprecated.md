

- ClockKit
- CLKRelativeDateTextProvider
-  date Deprecated

Instance Property

# date

The target date to use for calculations.

watchOS 2.0–9.0Deprecated

``` source
var date: Date { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

When creating a text provider that updates automatically, the provider calculates the relative date between this property and the current date. The value of this property must not be `nil`.

When creating a fixed, relative text provider, the provider calculates the relative date between this property and the relativeToDate property.

## See Also

### Getting the Date Information

var relativeToDate: Date?

The end date that the text provider uses when calculating a fixed, relative date.

Deprecated

var relativeDateStyle: CLKRelativeDateStyle

The formatting style to use for the relative time value.

Deprecated

var calendarUnits: NSCalendar.Unit

The calendar units to include in the formatted string.

Deprecated

