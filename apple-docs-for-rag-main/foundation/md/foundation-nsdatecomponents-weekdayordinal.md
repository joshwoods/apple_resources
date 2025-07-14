

- Foundation
- NSDateComponents
-  weekdayOrdinal 

Instance Property

# weekdayOrdinal

The ordinal number of weekdays.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var weekdayOrdinal: Int { get set }
```

## Discussion

Weekday ordinal units represent the position of the weekday within the next larger calendar unit, such as the month. For example, *2* is the weekday ordinal unit for the *second* Friday of the month.

This value is interpreted in the context of the calendar with which it is used—see Calendars, Date Components, and Calendar Units in Date and Time Programming Guide.

## See Also

### Accessing Weeks and Days

var weekday: Int

The number of the weekdays.

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

