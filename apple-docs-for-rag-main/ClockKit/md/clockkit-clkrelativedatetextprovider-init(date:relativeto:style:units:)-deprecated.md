

- ClockKit
- CLKRelativeDateTextProvider
-  init(date:relativeTo:style:units:) Deprecated

Initializer

# init(date:relativeTo:style:units:)

Creates a text provider that shows the difference in time between the provided dates.

watchOS 7.0–9.0Deprecated

``` source
convenience init(
    date: Date,
    relativeTo relativeToDate: Date?,
    style: CLKRelativeDateStyle,
    units calendarUnits: NSCalendar.Unit
)
```

## Parameters 

`date`  

The starting date, used to calculate the relative date string.

`relativeToDate`  

The end date, used to calculate the relative date string.

`style`  

The style to use when formatting the relative date value. For a list of possible values, see CLKRelativeDateStyle.

`calendarUnits`  

The units to include in the resulting date string. For a list of supported calendar units, see Date Format Options.

## Discussion

This initializer creates a text provider that produces a fixed, relative date. If you want a text provider that automatically updates as time passes, use init(date:style:units:) instead.

## See Also

### Creating a Text Provider

convenience init(date: Date, style: CLKRelativeDateStyle, units: NSCalendar.Unit)

Creates a text provider that shows the difference between the current time and the specified date.

Deprecated

