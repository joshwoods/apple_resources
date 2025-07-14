

- ClockKit
- CLKRelativeDateTextProvider
-  init(date:style:units:) Deprecated

Initializer

# init(date:style:units:)

Creates a text provider that shows the difference between the current time and the specified date.

watchOS 2.0–9.0Deprecated

``` source
convenience init(
    date: Date,
    style: CLKRelativeDateStyle,
    units calendarUnits: NSCalendar.Unit
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`date`  

The date to use for calculations. This parameter must not be `nil`.

`style`  

The style to use when formatting the relative date value. For a list of possible values, see CLKRelativeDateStyle.

`calendarUnits`  

The units to include in the resulting date string. For a list of supported calendar units, see Date Format Options.

## Discussion

This initializer produces a text provider that updates automatically as time passes. To create a text provider that produces a static, relative date, use init(date:relativeTo:style:units:) instead.

The text provider created by this method uses the default time zone information for the current user. The system formats date values according to the user’s current locale information.

## See Also

### Creating a Text Provider

convenience init(date: Date, relativeTo: Date?, style: CLKRelativeDateStyle, units: NSCalendar.Unit)

Creates a text provider that shows the difference in time between the provided dates.

Deprecated

