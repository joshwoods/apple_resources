

- Foundation
- Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
-  Date.FormatStyle.Symbol.TimeZone 

Structure

# Date.FormatStyle.Symbol.TimeZone

A type that specifies a format for the time zone in a date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct TimeZone
```

## Overview

The type Date.FormatStyle.Symbol.TimeZone includes static factory variables and methods that create custom Date.FormatStyle.Symbol.TimeZone objects:

| Factory variable | Description |
|----|----|
| specificName(_:) | The specific, non-location representation of a timezone. For example, `CDT` (`short`), `Central Daylight Time` (`long`). |
| genericName(_:) | The generic, non-location representation of a timezone. For example, `CT` (`short`), `Central Time` (`long`). |
| iso8601(_:) | The ISO 8601 representation of the timezone with hours, minutes, and optional seconds. For example, `-0500` (`short`), `-05:00` (`long`). |
| localizedGMT(_:) | The localized GMT format representation of a timezone. For example, `GMT-5` (`short`), `GMT-05:00` (`long`). |
| identifier(_:) | The timezone identifier. For example, `uschi` (`short`), `America/Chicago` (`long`). |
| exemplarLocation | The exemplar city for a timezone. For example, `Chicago`. |
| genericLocation | The generic location representation of a timezone. For example, `Chicago Time`. |

To customize the hour format in a string representation of a `Date`, use timeZone(_:). The following example shows a variety of Date.FormatStyle.Symbol.TimeZone format styles applied to a date.

```
let meetingDate = Date() // Feb 9, 2021 at 7:00 PM

meetingDate.formatted(Date.FormatStyle().timeZone(.specificName(.short)))
// CDT
meetingDate.formatted(Date.FormatStyle().timeZone(.specificName(.long)))
// Central Daylight Time

meetingDate.formatted(Date.FormatStyle().timeZone(.genericName(.short)))
// CT
meetingDate.formatted(Date.FormatStyle().timeZone(.genericName(.long)))
// Central Time

meetingDate.formatted(Date.FormatStyle().timeZone(.iso8601(.short)))
// -0500
meetingDate.formatted(Date.FormatStyle().timeZone(.iso8601(.long)))
// -05:00

meetingDate.formatted(Date.FormatStyle().timeZone(.localizedGMT(.short)))
// GMT-5
meetingDate.formatted(Date.FormatStyle().timeZone(.localizedGMT(.long)))
// GMT-05:00

meetingDate.formatted(Date.FormatStyle().timeZone(.identifier(.short)))
// uschi
meetingDate.formatted(Date.FormatStyle().timeZone(.identifier(.long)))
// America/Chicago

meetingDate.formatted(Date.FormatStyle().timeZone(.exemplarLocation))
// Chicago

meetingDate.formatted(Date.FormatStyle().timeZone(.genericLocation))
// Chicago Time

```

If you don’t provide a format, the system formats a timezone using the short specificName(_:) static function with the width Date.FormatStyle.Symbol.TimeZone.Width.short.

For more information about formatting dates, see the Date.FormatStyle.

## Topics

### Modifying a Time Zone

static func specificName(Date.FormatStyle.Symbol.TimeZone.Width) -> Date.FormatStyle.Symbol.TimeZone

Returns the specific, non-location representation of a timezone.

static func genericName(Date.FormatStyle.Symbol.TimeZone.Width) -> Date.FormatStyle.Symbol.TimeZone

Returns the generic, non-location representation of a timezone.

static func iso8601(Date.FormatStyle.Symbol.TimeZone.Width) -> Date.FormatStyle.Symbol.TimeZone

Creates the ISO 8601 representation of the timezone with hours, minutes, and optional seconds.

static func localizedGMT(Date.FormatStyle.Symbol.TimeZone.Width) -> Date.FormatStyle.Symbol.TimeZone

Returns the localized GMT format representation of a timezone.

static func identifier(Date.FormatStyle.Symbol.TimeZone.Width) -> Date.FormatStyle.Symbol.TimeZone

Returns the timezone identifier.

static var exemplarLocation: Date.FormatStyle.Symbol.TimeZone

The exemplar city for a timezone.

static var genericLocation: Date.FormatStyle.Symbol.TimeZone

The generic location representation of a timezone.

### Comparing Time Zones

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Supporting Enumerations

enum Width

A type representing the width of a timezone in a format style.

### Type Properties

static let omitted: Date.FormatStyle.Symbol.TimeZone

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

struct VerbatimHour

A type that specifies a format for the hour in a date format style.

