

- Foundation
- NSCalendar
-  NSCalendar.Unit 

Structure

# NSCalendar.Unit

Calendrical units such as year, month, day and hour.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Unit
```

## Overview

Calendar units may be used as a bit mask to specify a combination of units. Values in this enumeration are equal to the corresponding constants in `CFCalendarUnit`.

## Topics

### Initializers

init(rawValue: UInt)

### Specifying Years and Months

static var era: NSCalendar.Unit

Identifier for the era unit.

static var year: NSCalendar.Unit

Identifier for the year unit.

static var yearForWeekOfYear: NSCalendar.Unit

Identifier for the week-counting year unit.

static var quarter: NSCalendar.Unit

Identifier for the quarter of the calendar.

static var month: NSCalendar.Unit

Identifier for the month unit.

static var era: NSCalendar.Unit

Identifier for the era unit.

static var year: NSCalendar.Unit

Identifier for the year unit.

static var yearForWeekOfYear: NSCalendar.Unit

Identifier for the week-counting year unit.

static var quarter: NSCalendar.Unit

Identifier for the quarter of the calendar.

static var month: NSCalendar.Unit

Identifier for the month unit.

### Specifying Weeks and Days

static var weekOfYear: NSCalendar.Unit

Identifier for the week of the year calendar unit.

static var weekOfMonth: NSCalendar.Unit

Identifier for the week of the month calendar unit.

static var weekday: NSCalendar.Unit

Identifier for the weekday unit.

static var weekdayOrdinal: NSCalendar.Unit

Identifier for the ordinal weekday unit.

static var day: NSCalendar.Unit

Identifier for the day unit.

static var weekOfYear: NSCalendar.Unit

Identifier for the week of the year calendar unit.

static var weekOfMonth: NSCalendar.Unit

Identifier for the week of the month calendar unit.

static var weekday: NSCalendar.Unit

Identifier for the weekday unit.

static var weekdayOrdinal: NSCalendar.Unit

Identifier for the ordinal weekday unit.

static var day: NSCalendar.Unit

Identifier for the day unit.

### Specifying Hours, Minutes, and Seconds

static var hour: NSCalendar.Unit

Identifier for the hour unit.

static var minute: NSCalendar.Unit

Identifier for the minute unit.

static var second: NSCalendar.Unit

Identifier for the second unit.

static var nanosecond: NSCalendar.Unit

Identifier for the nanosecond unit.

static var hour: NSCalendar.Unit

Identifier for the hour unit.

static var minute: NSCalendar.Unit

Identifier for the minute unit.

static var second: NSCalendar.Unit

Identifier for the second unit.

static var nanosecond: NSCalendar.Unit

Identifier for the nanosecond unit.

### Specifying Calendars and Time Zones

static var calendar: NSCalendar.Unit

Identifier for the calendar of a date components object.

static var timeZone: NSCalendar.Unit

Identifier for the time zone of a date components object.

static var calendar: NSCalendar.Unit

Identifier for the calendar of a date components object.

static var timeZone: NSCalendar.Unit

Identifier for the time zone of a date components object.

### Deprecated

static var NSEraCalendarUnit: NSCalendar.Unit

Specifies the era unit.

Deprecated

static var NSYearCalendarUnit: NSCalendar.Unit

Specifies the year unit.

Deprecated

static var NSMonthCalendarUnit: NSCalendar.Unit

Specifies the month unit.

Deprecated

static var NSDayCalendarUnit: NSCalendar.Unit

Specifies the day unit.

Deprecated

static var NSHourCalendarUnit: NSCalendar.Unit

Specifies the hour unit.

Deprecated

static var NSMinuteCalendarUnit: NSCalendar.Unit

Specifies the minute unit.

Deprecated

static var NSSecondCalendarUnit: NSCalendar.Unit

Specifies the second unit.

Deprecated

static var NSWeekCalendarUnit: NSCalendar.Unit

Specifies the week unit.

Deprecated

static var NSWeekdayCalendarUnit: NSCalendar.Unit

Specifies the weekday unit.

Deprecated

static var NSWeekdayOrdinalCalendarUnit: NSCalendar.Unit

Specifies the ordinal weekday unit.

Deprecated

static var NSQuarterCalendarUnit: NSCalendar.Unit

Specifies the quarter of the calendar as a second. In macOS 10.6 and earlier this was defined as equal to quarter. In macOS 10.7 and later it is defined as `(1 

Deprecated

static var NSWeekOfMonthCalendarUnit: NSCalendar.Unit

Specifies the original week of a month calendar unit.

Deprecated

static var NSWeekOfYearCalendarUnit: NSCalendar.Unit

Specifies the original week of the year calendar unit.

Deprecated

static var NSYearForWeekOfYearCalendarUnit: NSCalendar.Unit

Specifies the year when the calendar is being interpreted as a week-based calendar.

Deprecated

static var NSCalendarCalendarUnit: NSCalendar.Unit

Specifies the calendar of the calendar.

Deprecated

static var NSTimeZoneCalendarUnit: NSCalendar.Unit

Specifies the time zone of the calendar as an `NSTimeZone`.

Deprecated

static var NSEraCalendarUnit: NSCalendar.Unit

Specifies the era unit.

Deprecated

static var NSYearCalendarUnit: NSCalendar.Unit

Specifies the year unit.

Deprecated

static var NSMonthCalendarUnit: NSCalendar.Unit

Specifies the month unit.

Deprecated

static var NSDayCalendarUnit: NSCalendar.Unit

Specifies the day unit.

Deprecated

static var NSHourCalendarUnit: NSCalendar.Unit

Specifies the hour unit.

Deprecated

static var NSMinuteCalendarUnit: NSCalendar.Unit

Specifies the minute unit.

Deprecated

static var NSSecondCalendarUnit: NSCalendar.Unit

Specifies the second unit.

Deprecated

static var NSWeekCalendarUnit: NSCalendar.Unit

Specifies the week unit.

Deprecated

static var NSWeekdayCalendarUnit: NSCalendar.Unit

Specifies the weekday unit.

Deprecated

static var NSWeekdayOrdinalCalendarUnit: NSCalendar.Unit

Specifies the ordinal weekday unit.

Deprecated

static var NSQuarterCalendarUnit: NSCalendar.Unit

Specifies the quarter of the calendar as a second. In macOS 10.6 and earlier this was defined as equal to quarter. In macOS 10.7 and later it is defined as `(1 

Deprecated

static var NSWeekOfMonthCalendarUnit: NSCalendar.Unit

Specifies the original week of a month calendar unit.

Deprecated

static var NSWeekOfYearCalendarUnit: NSCalendar.Unit

Specifies the original week of the year calendar unit.

Deprecated

static var NSYearForWeekOfYearCalendarUnit: NSCalendar.Unit

Specifies the year when the calendar is being interpreted as a week-based calendar.

Deprecated

static var NSCalendarCalendarUnit: NSCalendar.Unit

Specifies the calendar of the calendar.

Deprecated

static var NSTimeZoneCalendarUnit: NSCalendar.Unit

Specifies the time zone of the calendar as an `NSTimeZone`.

Deprecated

### Type Properties

static var dayOfYear: NSCalendar.Unit

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Getting Calendar Information

var calendarIdentifier: NSCalendar.Identifier

An identifier for the calendar.

var firstWeekday: Int

The index of the first weekday of the receiver.

var locale: Locale?

The locale of the receiver.

var timeZone: TimeZone

The time zone for the calendar.

func maximumRange(of: NSCalendar.Unit) -> NSRange

Returns the maximum range limits of the values that a given unit can take on.

func minimumRange(of: NSCalendar.Unit) -> NSRange

Returns the minimum range limits of the values that a given unit can take on.

var minimumDaysInFirstWeek: Int

The minimum number of days in the first week of the receiver.

func ordinality(of: NSCalendar.Unit, in: NSCalendar.Unit, for: Date) -> Int

Returns, for a given absolute time, the ordinal number of a smaller calendar unit (such as a day) within a specified larger calendar unit (such as a week).

func range(of: NSCalendar.Unit, in: NSCalendar.Unit, for: Date) -> NSRange

Returns the range of absolute time values that a smaller calendar unit (such as a day) can take on in a larger calendar unit (such as a month) that includes a specified absolute time.

func range(of: NSCalendar.Unit, start: AutoreleasingUnsafeMutablePointer&lt;NSDate?>?, interval: UnsafeMutablePointer&lt;TimeInterval>?, for: Date) -> Bool

Returns by reference the starting time and duration of a given calendar unit that contains a given date.

func range(ofWeekendStart: AutoreleasingUnsafeMutablePointer&lt;NSDate?>?, interval: UnsafeMutablePointer&lt;TimeInterval>?, containing: Date) -> Bool

Returns whether a given date falls within a weekend period, and if so, returns by reference the start date and time interval of the weekend range.

