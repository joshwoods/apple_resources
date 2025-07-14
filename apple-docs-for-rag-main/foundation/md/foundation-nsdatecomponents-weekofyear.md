

- Foundation
- NSDateComponents
-  weekOfYear 

Instance Property

# weekOfYear

The ISO 8601 week date of the year.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var weekOfYear: Int { get set }
```

## Discussion

This value is interpreted in the context of the calendar with which it is used—see Calendars, Date Components, and Calendar Units in Date and Time Programming Guide.

## See Also

### Related Documentation

var yearForWeekOfYear: Int

The ISO 8601 week-numbering year.

### Accessing Weeks and Days

var weekday: Int

The number of the weekdays.

var weekdayOrdinal: Int

The ordinal number of weekdays.

var weekOfMonth: Int

The week number of the months.

var day: Int

The number of days.

func week() -> Int

Returns the number of weeks.

Deprecated

func setWeek(Int)

Sets the number of weeks.

Deprecated

