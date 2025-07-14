

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.Day 

Structure

# Date.FormatStyle.Symbol.Day

A type that specifies the format for a day in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Day
```

## Overview

The Date.FormatStyle.Symbol.Day type includes static factory variables and methods that create custom Date.FormatStyle.Symbol.Day objects:

| Factory variable | Description |
|----|----|
| defaultDigits | The minimum number of digits that shows the numeric day of month. For example, `1`, `18`. |
| julianModified(minimumLength:) | The modified Julian day. The field length specifies the minimum number of digits, zero-padded if necessary. For example, `2451334`. |
| ordinalOfDayInMonth | The ordinal of the day in the month. For example, the second Wednesday in July would yield `2`. |
| twoDigits | The two-digit numeric day of month, zero-padded if necessary. For example, `01`, `18`. |

To customize the day format in a string representation of a `Date`, use day(_:). The following example shows a variety of Date.FormatStyle.Symbol.Day formats applied to a date.

```
let meetingDate = Date() // Feb 9, 2021 at 3:00 PM
meetingDate.formatted(Date.FormatStyle().day(.defaultDigits)) // 9
meetingDate.formatted(Date.FormatStyle().day(.ordinalOfDayInMonth)) // 2 (second Tuesday of the month)
meetingDate.formatted(Date.FormatStyle().day(.twoDigits)) // 09
meetingDate.formatted(Date.FormatStyle().day(.julianModified(minimumLength: 12))) // 0002459255
meetingDate.formatted(Date.FormatStyle().day()) // 9
```

If no format is specified as a parameter, the defaultDigits static variable is the default format.

For more information about formatting dates, see the Date.FormatStyle.

## Topics

### Modifying a Day Format

static var defaultDigits: Date.FormatStyle.Symbol.Day

Custom format style portraying the minimum number of digits that represents the numeric day of month.

static var ordinalOfDayInMonth: Date.FormatStyle.Symbol.Day

Custom format style portraying the ordinal of the day in the month.

static var twoDigits: Date.FormatStyle.Symbol.Day

Custom format style portraying the two-digit numeric day of month, zero-padded if necessary.

static func julianModified(minimumLength: Int) -> Date.FormatStyle.Symbol.Day

Creates a custom day format style representing the modified Julian day.

### Comparing Day Formats

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.Day

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Modifying Date Style Format Symbols

struct CyclicYear

A type that specifies a format for a cyclic year in a date format style.

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

struct VerbatimHour

A type that specifies a format for the hour in a date format style.

