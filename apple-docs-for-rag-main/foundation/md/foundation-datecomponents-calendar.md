

- Foundation
- DateComponents
-  calendar 

Instance Property

# calendar

The calendar used to interpret the other values in this structure.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var calendar: Calendar? { get set }
```

## Discussion

Note

API which uses `DateComponents` may have different behavior if this value is `nil`. For example, assuming the current calendar or ignoring certain values.

## See Also

### Initializing Date Components

init(calendar: Calendar?, timeZone: TimeZone?, era: Int?, year: Int?, month: Int?, day: Int?, hour: Int?, minute: Int?, second: Int?, nanosecond: Int?, weekday: Int?, weekdayOrdinal: Int?, quarter: Int?, weekOfMonth: Int?, weekOfYear: Int?, yearForWeekOfYear: Int?)

Initializes a date components value, optionally specifying values for its fields.

var timeZone: TimeZone?

A time zone.

