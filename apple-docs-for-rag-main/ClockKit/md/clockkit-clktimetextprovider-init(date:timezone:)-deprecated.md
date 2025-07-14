

- ClockKit
- CLKTimeTextProvider
-  init(date:timeZone:) Deprecated

Initializer

# init(date:timeZone:)

Creates and returns a text provider for displaying the specified time.

watchOS 2.0–9.0Deprecated

``` source
convenience init(
    date: Date,
    timeZone: TimeZone?
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`date`  

The date object containing the time to display. This parameter must not be `nil`.

`timeZone`  

The time zone to use when formatting the date. If you specify `nil`, the text provider uses the default time zone currently associated with the user.

## Return Value

A text provider initialized with the specified date and time zone value.

## See Also

### Creating a Text Provider

convenience init(date: Date)

Creates and returns a text provider for displaying the specified time.

Deprecated

