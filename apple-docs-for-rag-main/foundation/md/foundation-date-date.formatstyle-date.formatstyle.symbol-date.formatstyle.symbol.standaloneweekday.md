

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.StandaloneWeekday 

Structure

# Date.FormatStyle.Symbol.StandaloneWeekday

A type that specifies the format for a standalone weekday.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct StandaloneWeekday
```

## Topics

### Modifying a Standalone Weekday

static var abbreviated: Date.FormatStyle.Symbol.StandaloneWeekday

The abbreviated representation of a standalone weekday.

static var narrow: Date.FormatStyle.Symbol.StandaloneWeekday

The shortest representation of a standalone weekday.

static var oneDigit: Date.FormatStyle.Symbol.StandaloneWeekday

The one-digit representation of a standalone weekday.

static var short: Date.FormatStyle.Symbol.StandaloneWeekday

The short representation of a standalone weekday.

static var wide: Date.FormatStyle.Symbol.StandaloneWeekday

The full representation of a standalone weekday.

### Comparing Standalone Weekdays

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

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

struct TimeZone

A type that specifies a format for the time zone in a date format style.

struct VerbatimHour

A type that specifies a format for the hour in a date format style.

