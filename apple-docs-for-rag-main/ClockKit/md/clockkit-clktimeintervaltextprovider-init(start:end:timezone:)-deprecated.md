

- ClockKit
- CLKTimeIntervalTextProvider
-  init(start:end:timeZone:) Deprecated

Initializer

# init(start:end:timeZone:)

Creates and returns a text provider with the specified dates and time zone information.

watchOS 2.0–9.0Deprecated

``` source
convenience init(
    start startDate: Date,
    end endDate: Date,
    timeZone: TimeZone?
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`startDate`  

The start date for the time range. This parameter must not be `nil`.

`endDate`  

The end date for the time range. The specified date must come after the date in the `startDate` parameter. This parameter must not be `nil`.

`timeZone`  

The time zone to use when formatting dates. If you specify `nil`, the text provider uses the time zone currently associated with the user.

## Return Value

A text provider initialized with the specified date and time zone values.

## Discussion

The returned text provider uses the default calendar information for the current user and uses the time zone in the `timeZone` parameter. Date and time values are formatted according to the user’s current locale information.

## See Also

### Creating the Text Provider

convenience init(start: Date, end: Date)

Creates and returns a text provider with the specified start and end dates.

Deprecated

