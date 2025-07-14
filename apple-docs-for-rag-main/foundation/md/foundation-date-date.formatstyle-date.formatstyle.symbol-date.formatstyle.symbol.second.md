

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.Second 

Structure

# Date.FormatStyle.Symbol.Second

A type that specifies the format for the seconds in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Second
```

## Overview

The type Date.FormatStyle.Symbol.Second includes static factory variables that create custom Date.FormatStyle.Symbol.Second objects:

| Factory variable | Description |
|----|----|
| defaultDigits | The minimum number of digits that represents the numeric second. For example, `1`, `18`. |
| twoDigits | Two-digit numeric second, zero-padded if necessary. For example, `01`, `18`. |

To customize the second format in a string representation of a `Date`, use second(_:). The following example shows a variety of Date.FormatStyle.Symbol.Second format styles applied to a date.

```
let meetingDate = Date() // Feb 9, 2021 at 3:05 PM
meetingDate.formatted(Date.FormatStyle().second(.defaultDigits)) // 5
meetingDate.formatted(Date.FormatStyle().second(.twoDigits)) // 05
meetingDate.formatted(Date.FormatStyle().second()) // 5
```

If no format is specified as a parameter, the defaultDigits static variable is the default format.

For more information about formatting dates, see the Date.FormatStyle.

## Topics

### Modifying a Second

static var defaultDigits: Date.FormatStyle.Symbol.Second

The custom format style that conveys the minimum number of digits that represents the numeric second.

static var twoDigits: Date.FormatStyle.Symbol.Second

The custom format style that conveys a two-digit numeric second, zero-padded if necessary.

### Comparing Seconds

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.Second

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

