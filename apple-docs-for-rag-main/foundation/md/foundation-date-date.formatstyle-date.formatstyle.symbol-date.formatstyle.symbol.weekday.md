

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.Weekday 

Structure

# Date.FormatStyle.Symbol.Weekday

A type that specifies the format for the weekday name in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Weekday
```

## Overview

The type Date.FormatStyle.Symbol.Weekday includes static factory variables that create custom Date.FormatStyle.Symbol.Weekday objects:

| Factory variable | Description |
|----|----|
| abbreviated | Abbreviated weekday name. For example, `Tue`. |
| wide | Wide weekday name. For example, `Tuesday`. |
| narrow | Narrow weekday name. For example, `T`. |
| short | Short weekday name. For example, `Tu`. |
| oneDigit | Local numeric one-digit day of week. The value depends on the local starting day of the week. For example, this is `2` if Sunday is the first day of the week. |
| twoDigits | Local numeric two-digit day of week, zero-padded if necessary. The value depends on the local starting day of the week. For example, this is `02` if Sunday is the first day of the week. |

To customize the weekday, name format in a string representation of a `Date`, use weekday(_:). This example shows a variety of Date.FormatStyle.Symbol.Weekday format styles applied to a Thursday, using locale `en_US`:

```
let meetingDate = Date() // Feb 18, 2021 at 3:00 PM
meetingDate.formatted(Date.FormatStyle().weekday(.abbreviated)) // Thu
meetingDate.formatted(Date.FormatStyle().weekday(.narrow)) // T
meetingDate.formatted(Date.FormatStyle().weekday(.short)) // Th
meetingDate.formatted(Date.FormatStyle().weekday(.wide)) // Thursday
meetingDate.formatted(Date.FormatStyle().weekday(.oneDigit)) // 5
meetingDate.formatted(Date.FormatStyle().weekday(.twoDigits)) // 05
meetingDate.formatted(Date.FormatStyle().weekday()) // Thu
```

If no format is specified as a parameter, the abbreviated static variable is the default format.

For more information about formatting dates, see the Date.FormatStyle.

## Topics

### Modifying a Weekday

static var abbreviated: Date.FormatStyle.Symbol.Weekday

A shortened weekday representation.

static var narrow: Date.FormatStyle.Symbol.Weekday

The shortest weekday representation.

static var oneDigit: Date.FormatStyle.Symbol.Weekday

The one-digit representation of a weekday.

static var short: Date.FormatStyle.Symbol.Weekday

The short weekday representation.

static var twoDigits: Date.FormatStyle.Symbol.Weekday

The two-digit representation of a standalone weekday, zero-padded if necessary.

static var wide: Date.FormatStyle.Symbol.Weekday

The complete weekday representation.

### Comparing a Weekday

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.Weekday

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

