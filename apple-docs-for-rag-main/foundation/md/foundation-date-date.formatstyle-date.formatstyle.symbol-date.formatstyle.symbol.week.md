

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.Week 

Structure

# Date.FormatStyle.Symbol.Week

A type that specifies the format for the week in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Week
```

## Overview

The type Date.FormatStyle.Symbol.Week includes static factory variables that create custom Date.FormatStyle.Symbol.Week objects:

| Factory variable | Description |
|----|----|
| defaultDigits | The minimum number of digits that represents the full numeric week. For example, `1`, `18`. |
| twoDigits | Two-digit numeric week, zero-padded if necessary. For example, `01`, `18`. |
| weekOfMonth | The numeric week of the month. For example, `1`, `4`. |

To customize the week format in a string representation of a `Date`, use week(_:). The following example shows a variety of Date.FormatStyle.Symbol.Week format styles applied to a date.

```
let meetingDate = Date() // May 3, 2021 at 3:00 PM
meetingDate.formatted(Date.FormatStyle().week(.defaultDigits)) // 19
meetingDate.formatted(Date.FormatStyle().week(.twoDigits)) // 19
meetingDate.formatted(Date.FormatStyle().week(.weekOfMonth)) // 2
meetingDate.formatted(Date.FormatStyle().week()) // 19

```

An incomplete week at the start of a month is week of the month `1`. If no format is specified as a parameter, the defaultDigits static variable is the default format.

For more information about formatting dates, see the Date.FormatStyle.

## Topics

### Modifying a Week

static var defaultDigits: Date.FormatStyle.Symbol.Week

Custom week format style showing the minimum number of digits that represents the numeric week.

static var twoDigits: Date.FormatStyle.Symbol.Week

Custom format style portraying the two-digit numeric week, zero-padded if necessary.

static var weekOfMonth: Date.FormatStyle.Symbol.Week

Custom format style portraying the numeric week of the month.

### Comparing Weeks

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.Week

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

