

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.Month 

Structure

# Date.FormatStyle.Symbol.Month

A type that specifies a format for the month in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Month
```

## Overview

The type Date.FormatStyle.Symbol.Month includes static factory variables that create custom Date.FormatStyle.Symbol.Month objects:

| Factory variable | Description |
|----|----|
| abbreviated | Abbreviated month name. For example, `Sep`. |
| defaultDigits | Minimum number of digits that represents the numeric month. For example, `9`, `12`. |
| narrow | Narrow month name. For example, `S`. |
| twoDigits | Two-digit numeric month, zero-padded if necessary. For example, `09`, `12`. |
| wide | Wide month name. For example, `September`. |

To customize the month format in a string representation of a `Date`, use month(_:). The following example shows a variety of Date.FormatStyle.Symbol.Month format styles applied to a date.

```
let meetingDate = Date() // Feb 9, 2021 at 3:00 PM
meetingDate.formatted(Date.FormatStyle().month(.abbreviated)) // Feb
meetingDate.formatted(Date.FormatStyle().month(.narrow)) // F
meetingDate.formatted(Date.FormatStyle().month(.defaultDigits)) // 2
meetingDate.formatted(Date.FormatStyle().month(.twoDigits)) // 02
meetingDate.formatted(Date.FormatStyle().month(.wide)) // February
meetingDate.formatted(Date.FormatStyle().month()) // Feb
```

If no format is specified as a parameter, the abbreviated static variable is the default format.

For more information about formatting dates, see the Date.FormatStyle.

## Topics

### Modifying a Month

static var abbreviated: Date.FormatStyle.Symbol.Month

The abbreviated representation of a month.

static var defaultDigits: Date.FormatStyle.Symbol.Month

Custom month format style showing the minimum number of digits that represents the numeric month.

static var narrow: Date.FormatStyle.Symbol.Month

The shortest representation of a month.

static var twoDigits: Date.FormatStyle.Symbol.Month

The custom month format style that uses two digits to represent the numeric month.

static var wide: Date.FormatStyle.Symbol.Month

The full representation of a month.

### Comparing a Month

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.Month

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

struct VerbatimHour

A type that specifies a format for the hour in a date format style.

