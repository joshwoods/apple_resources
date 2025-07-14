

- ClockKit
- CLKDateTextProvider
-  init(date:units:timeZone:) Deprecated

Initializer

# init(date:units:timeZone:)

Creates and returns a text provider with the specified date and time zone.

watchOS 2.0–9.0Deprecated

``` source
convenience init(
    date: Date,
    units calendarUnits: NSCalendar.Unit,
    timeZone: TimeZone?
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`date`  

The date to display. This parameter must not be `nil`.

`calendarUnits`  

The units to include in the resulting date string. For a list of supported calendar units, see Date Format Options.

`timeZone`  

The time zone to use when formatting the date. If you specify `nil`, the text provider uses the time zone currently associated with the user.

## Return Value

A text provider initialized with the specified date and time zone information.

## Discussion

Date values are formatted according to the user’s current locale information.

## See Also

### Creating a Text Provider

convenience init(date: Date, units: NSCalendar.Unit)

Creates and returns a text provider with the specified date and the default time zone.

Deprecated

