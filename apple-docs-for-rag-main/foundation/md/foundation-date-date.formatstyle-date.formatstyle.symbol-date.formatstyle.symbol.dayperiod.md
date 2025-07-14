

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.DayPeriod 

Structure

# Date.FormatStyle.Symbol.DayPeriod

A type that specifies a format for the time period in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct DayPeriod
```

## Overview

The type Date.FormatStyle.Symbol.DayPeriod includes static factory methods that create custom Date.FormatStyle.Symbol.DayPeriod objects.

| Factory variable | Description |
|----|----|
| conversational(_:) | Conversational abbreviated period. For example, `at night`, `nachm.`, `iltap`.  Conversational narrow period. For example, `at night`, `nachmittags`, `iltapäivällä`.  Conversational wide period. For example, `at night`, `nachm.`, `ip.` |
| standard(_:) | Abbreviated period. For example, `am`.  Narrow period. For example, `a`.  Wide period. For example, `am`. |
| with12s(_:) | Abbreviated period including designations for noon and midnight. For example, `mid.`  Narrow period including designations for noon and midnight. For example, `md`.  Wide period including designations for noon and midnight. For example, `midnight`. |

The day period format style may be uppercase or lowercase depending on the locale and other options.

For more information about formatting dates, see the Date.FormatStyle.

## Topics

### Modifying a Day Period

static func conversational(Date.FormatStyle.Symbol.DayPeriod.Width) -> Date.FormatStyle.Symbol.DayPeriod

Static factory method that creates a custom day period format style using a conversational style.

static func standard(Date.FormatStyle.Symbol.DayPeriod.Width) -> Date.FormatStyle.Symbol.DayPeriod

Static factory method that creates a custom day period format style using a standard style.

static func with12s(Date.FormatStyle.Symbol.DayPeriod.Width) -> Date.FormatStyle.Symbol.DayPeriod

Static factory method that creates a custom day period format style using a style that represents midday and midnight.

### Supporting Enumerations

enum Width

A type representing the width of a day period in a format style.

### Comparing Day Periods

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.DayPeriod

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

