

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.SecondFraction 

Structure

# Date.FormatStyle.Symbol.SecondFraction

A type that specifies the format for the second fraction in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SecondFraction
```

## Overview

The type Date.FormatStyle.Symbol.SecondFraction includes static factory methods that create custom Date.FormatStyle.Symbol.SecondFraction objects:

| Factory variable | Description |
|----|----|
| fractional(_:) | Returns the numerical representation of the fractional component of the second. For example, `8`, `827`. |
| milliseconds(_:) | Returns the number of milliseconds elapsed in the day. For example, `11122827`. |

To customize the second format in a string representation of a `Date`, use secondFraction(_:). The following example shows a variety of Date.FormatStyle.Symbol.SecondFraction format styles applied to a date.

```
let meetingDate = Date() // Feb 9, 2021 at 3:05:41 PM
meetingDate.formatted(Date.FormatStyle().secondFraction(.fractional(3))) // 827
meetingDate.formatted(Date.FormatStyle().secondFraction(.fractional(1))) // 8
meetingDate.formatted(Date.FormatStyle().secondFraction(.milliseconds(4))) // 11122827
```

For more information about formatting dates, see the Date.FormatStyle.

## Topics

### Modifying a Second Fraction

static func fractional(Int) -> Date.FormatStyle.Symbol.SecondFraction

Creates a custom format style representing the fractional seconds component of a date.

static func milliseconds(Int) -> Date.FormatStyle.Symbol.SecondFraction

Creates a custom format style representing the milliseconds elapsed in a day.

### Comparing Second Fractions

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.SecondFraction

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

