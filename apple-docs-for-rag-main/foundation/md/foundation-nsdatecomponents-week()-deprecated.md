

- Foundation
- NSDateComponents
-  week() Deprecated

Instance Method

# week()

Returns the number of weeks.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func week() -> Int
```

Deprecated

Use weekOfYear or weekOfMonth instead, depending on what you intend.

## Return Value

The number of week units for the receiver.

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

var day: Int

The number of days.

func setWeek(Int)

Sets the number of weeks.

Deprecated

