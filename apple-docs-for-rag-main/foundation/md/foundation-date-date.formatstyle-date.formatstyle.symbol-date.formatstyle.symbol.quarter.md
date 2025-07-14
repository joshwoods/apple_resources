

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.Quarter 

Structure

# Date.FormatStyle.Symbol.Quarter

A type that specifies the format for the quarter in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Quarter
```

## Overview

The type Date.FormatStyle.Symbol.Quarter includes static factory variables that create custom Date.FormatStyle.Symbol.Quarter objects:

| Factory variable | Description |
|----|----|
| abbreviated | Abbreviated quarter name. For example, `Q2`. |
| narrow | Minimum number of digits that represents the numeric quarter. For example, `2`. |
| oneDigit | One-digit numeric quarter. For example, `1`, `4`. |
| twoDigits | Two-digit numeric quarter, zero-padded if necessary. For example, `01`, `04`. |
| wide | Wide quarter name. For example, `2nd quarter`. |

To customize the month format in a string representation of a `Date`, use quarter(_:). The following example shows a variety of Date.FormatStyle.Symbol.Quarter format styles applied to a date.

```
let meetingDate = Date() // Oct 7, 2020 at 3:00 PM
meetingDate.formatted(Date.FormatStyle().quarter(.abbreviated)) // Q4
meetingDate.formatted(Date.FormatStyle().quarter(.narrow)) // 4th quarter
meetingDate.formatted(Date.FormatStyle().quarter(.oneDigit)) // 4
meetingDate.formatted(Date.FormatStyle().quarter(.twoDigits)) // 04
meetingDate.formatted(Date.FormatStyle().quarter(.wide)) // 4th quarter
meetingDate.formatted(Date.FormatStyle().quarter()) // Q4

```

If no format is specified as a parameter, the abbreviated static variable is the default format.

For more information about formatting dates, see the Date.FormatStyle.

## Topics

### Modifying a Quarter

static var abbreviated: Date.FormatStyle.Symbol.Quarter

The abbreviated representation of a quarter.

static var narrow: Date.FormatStyle.Symbol.Quarter

The shortest representation of a quarter.

static var oneDigit: Date.FormatStyle.Symbol.Quarter

The one-digit representation of a quarter.

static var twoDigits: Date.FormatStyle.Symbol.Quarter

The two-digit representation of a quarter.

static var wide: Date.FormatStyle.Symbol.Quarter

The full representation of a quarter.

### Comparing Quarters

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.Quarter

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

