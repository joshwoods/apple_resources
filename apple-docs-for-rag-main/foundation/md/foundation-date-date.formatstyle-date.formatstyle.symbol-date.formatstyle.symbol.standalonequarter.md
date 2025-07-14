

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.StandaloneQuarter 

Structure

# Date.FormatStyle.Symbol.StandaloneQuarter

A type that specifies the format for a standalone quarter.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct StandaloneQuarter
```

## Topics

### Modifying a Standalone Quarter

static var abbreviated: Date.FormatStyle.Symbol.StandaloneQuarter

The abbreviated representation of a standalone quarter.

static var narrow: Date.FormatStyle.Symbol.StandaloneQuarter

The shortest representation of a standalone quarter.

static var oneDigit: Date.FormatStyle.Symbol.StandaloneQuarter

The one-digit representation of a standalone quarter.

static var twoDigits: Date.FormatStyle.Symbol.StandaloneQuarter

The two-digit representation of a standalone quarter.

static var wide: Date.FormatStyle.Symbol.StandaloneQuarter

The full representation of a standalone quarter.

### Comparing Standalone Quarters

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

struct StandaloneWeekday

A type that specifies the format for a standalone weekday.

struct TimeZone

A type that specifies a format for the time zone in a date format style.

struct VerbatimHour

A type that specifies a format for the hour in a date format style.

