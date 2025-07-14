

- Foundation
- NSDateComponents
-  day 

Instance Property

# day

The number of days.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var day: Int { get set }
```

## Discussion

This value is interpreted in the context of the calendar with which it is used—see Calendars, Date Components, and Calendar Units in Date and Time Programming Guide.

## See Also

### Accessing Weeks and Days

var weekday: Int

The number of the weekdays.

var weekdayOrdinal: Int

The ordinal number of weekdays.

var weekOfMonth: Int

The week number of the months.

var weekOfYear: Int

The ISO 8601 week date of the year.

func week() -> Int

Returns the number of weeks.

Deprecated

func setWeek(Int)

Sets the number of weeks.

Deprecated

