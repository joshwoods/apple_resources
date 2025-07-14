

- ClockKit
- CLKDateTextProvider
-  init(date:units:) Deprecated

Initializer

# init(date:units:)

Creates and returns a text provider with the specified date and the default time zone.

watchOS 2.0–9.0Deprecated

``` source
convenience init(
    date: Date,
    units calendarUnits: NSCalendar.Unit
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`date`  

The date to display. This parameter must not be `nil`.

`calendarUnits`  

The units to include in the resulting date string. For a list of supported calendar units, see Date Format Options.

## Return Value

A text provider initialized with the specified date and time zone information.

## Discussion

The text provider created by this method uses the default time zone information for the current user. Date values are formatted according to the user’s current locale information.

## See Also

### Creating a Text Provider

convenience init(date: Date, units: NSCalendar.Unit, timeZone: TimeZone?)

Creates and returns a text provider with the specified date and time zone.

Deprecated

