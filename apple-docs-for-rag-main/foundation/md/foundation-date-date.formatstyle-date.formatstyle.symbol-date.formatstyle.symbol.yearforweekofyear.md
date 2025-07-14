

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.YearForWeekOfYear 

Structure

# Date.FormatStyle.Symbol.YearForWeekOfYear

A type that specifies the format for a year in week-of-year calendars when you parse a string with a date format string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct YearForWeekOfYear
```

## Topics

### Modifying a Year for Week-of-Year

static var defaultDigits: Date.FormatStyle.Symbol.YearForWeekOfYear

Custom week of the year format style showing the minimum number of digits that represents the year in week-of-year calendars.

static var twoDigits: Date.FormatStyle.Symbol.YearForWeekOfYear

The custom format style that represents the two-digit numeric year in week-of-year calendars, zero-padded or truncated if necessary.

static func padded(Int) -> Date.FormatStyle.Symbol.YearForWeekOfYear

Returns a custom format style that represents the three or more digits of the year in week-of-year calendars, zero-padded if necessary.

### Comparing a Year for Week-of-Year

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.YearForWeekOfYear

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Modifying Date Style Format Symbols

struct CyclicYear

A type that specifies a format for a cyclic year in a date format style.

struct Day

A type that specifies the format for a day in a date format style.

struct DayOfYear

A type that specifies the format for the day of the year in a date format style.

struct DayPeriod

A type that specifies a format for the time period in a date format style.

struct Era

A type that specifies a format for the era in a date format style.

struct Hour

A type that specifies a format for the hour in a date format style.

struct Minute

A type that specifies the format for the minutes in a date format style.

struct Month

A type that specifies a format for the month in a date format style.

struct Quarter

A type that specifies the format for the quarter in a date format style.

struct Second

A type that specifies the format for the seconds in a date format style.

struct SecondFraction

A type that specifies the format for the second fraction in a date format style.

struct StandaloneMonth

A type that specifies the format for a standalone month.

struct StandaloneQuarter

A type that specifies the format for a standalone quarter.

struct StandaloneWeekday

A type that specifies the format for a standalone weekday.

struct TimeZone

A type that specifies a format for the time zone in a date format style.

