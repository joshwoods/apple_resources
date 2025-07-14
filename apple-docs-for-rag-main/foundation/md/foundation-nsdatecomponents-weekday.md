

- Foundation
- NSDateComponents
-  weekday 

Instance Property

# weekday

The number of the weekdays.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var weekday: Int { get set }
```

## Discussion

Weekday units are the numbers 1 through *n*, where *n* is the number of days in the week. For example, in the Gregorian calendar, *n* is 7 and Sunday is represented by 1.

This value is interpreted in the context of the calendar with which it is used—see Calendars, Date Components, and Calendar Units in Date and Time Programming Guide.

## See Also

### Accessing Weeks and Days

var weekdayOrdinal: Int

The ordinal number of weekdays.

var weekOfMonth: Int

The week number of the months.

var weekOfYear: Int

The ISO 8601 week date of the year.

var day: Int

The number of days.

func week() -> Int

Returns the number of weeks.

Deprecated

func setWeek(Int)

Sets the number of weeks.

Deprecated

