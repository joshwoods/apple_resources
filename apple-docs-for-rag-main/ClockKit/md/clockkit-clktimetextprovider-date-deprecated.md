

- ClockKit
- CLKTimeTextProvider
-  date Deprecated

Instance Property

# date

The date object containing the time value.

watchOS 2.0–9.0Deprecated

``` source
var date: Date { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

You can make changes to this property until you hand off the timeline entry containing it to ClockKit. The value of this property must not be `nil`.

## See Also

### Related Documentation

convenience init(date: Date)

Creates and returns a text provider for displaying the specified time.

Deprecated

convenience init(date: Date, timeZone: TimeZone?)

Creates and returns a text provider for displaying the specified time.

Deprecated

### Getting the Time Information

var timeZone: TimeZone?

The time zone used to format time values.

Deprecated

