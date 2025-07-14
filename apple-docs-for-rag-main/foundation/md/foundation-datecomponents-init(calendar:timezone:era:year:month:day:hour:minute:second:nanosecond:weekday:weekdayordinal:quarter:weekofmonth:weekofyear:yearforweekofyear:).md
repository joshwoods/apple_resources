

- Foundation
- DateComponents
-  init(calendar:timeZone:era:year:month:day:hour:minute:second:nanosecond:weekday:weekdayOrdinal:quarter:weekOfMonth:weekOfYear:yearForWeekOfYear:) 

Initializer

# init(calendar:timeZone:era:year:month:day:hour:minute:second:nanosecond:weekday:weekdayOrdinal:quarter:weekOfMonth:weekOfYear:yearForWeekOfYear:)

Initializes a date components value, optionally specifying values for its fields.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    calendar: Calendar? = nil,
    timeZone: TimeZone? = nil,
    era: Int? = nil,
    year: Int? = nil,
    month: Int? = nil,
    day: Int? = nil,
    hour: Int? = nil,
    minute: Int? = nil,
    second: Int? = nil,
    nanosecond: Int? = nil,
    weekday: Int? = nil,
    weekdayOrdinal: Int? = nil,
    quarter: Int? = nil,
    weekOfMonth: Int? = nil,
    weekOfYear: Int? = nil,
    yearForWeekOfYear: Int? = nil
)
```

## See Also

### Initializing Date Components

var calendar: Calendar?

The calendar used to interpret the other values in this structure.

var timeZone: TimeZone?

A time zone.

