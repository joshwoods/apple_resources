

- ClockKit
- CLKTimeTextProvider
-  timeZone Deprecated

Instance Property

# timeZone

The time zone used to format time values.

watchOS 2.0–9.0Deprecated

``` source
var timeZone: TimeZone? { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

If the value of this property is `nil`, the text provider uses the time zone currently configured for the user.

## See Also

### Related Documentation

convenience init(date: Date, timeZone: TimeZone?)

Creates and returns a text provider for displaying the specified time.

Deprecated

### Getting the Time Information

var date: Date

The date object containing the time value.

Deprecated

