

- ClockKit
- CLKTimeTextProvider
-  init(date:) Deprecated

Initializer

# init(date:)

Creates and returns a text provider for displaying the specified time.

watchOS 2.0–9.0Deprecated

``` source
convenience init(date: Date)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`date`  

The date object containing the time to display. This parameter must not be `nil`.

## Return Value

A text provider initialized with the specified date.

## Discussion

The text provider created by this method uses the default time zone information of the current user. The time value is formatted using the current locale information for the user.

## See Also

### Creating a Text Provider

convenience init(date: Date, timeZone: TimeZone?)

Creates and returns a text provider for displaying the specified time.

Deprecated

