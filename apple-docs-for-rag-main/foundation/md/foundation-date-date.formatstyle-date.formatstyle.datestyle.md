

- Foundation
- Date
- Date.FormatStyle
-  Date.FormatStyle.DateStyle 

Structure

# Date.FormatStyle.DateStyle

Type that defines date styles varied in length or components included.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct DateStyle
```

## Overview

The exact format depends on the locale. Possible values of date style include omitted, numeric, abbreviated, long, and complete.

The following code sample shows a variety of date style format results using the `en_US` locale.

```
let meetingDate = Date()
meetingDate.formatted(date: .omitted, time: .standard) 
// 9:42:14 AM

meetingDate.formatted(date: .numeric, time: .omitted) 
// 10/17/2020

meetingDate.formatted(date: .abbreviated, time: .omitted)
// Oct 17, 2020

meetingDate.formatted(date: .long, time: .omitted) 
// October 17, 2020

meetingDate.formatted(date: .complete, time: .omitted) 
// Saturday, October 17, 2020

meetingDate.formatted()
// 10/17/2020, 9:42 AM
```

The default date style is `numeric`.

## Topics

### Modifying a Date Style

static let abbreviated: Date.FormatStyle.DateStyle

A date style with some components abbreviated for space-constrained applications.

static let complete: Date.FormatStyle.DateStyle

A date style with all components represented.

static let long: Date.FormatStyle.DateStyle

A lengthened date style with the full month, day of month, and year components represented.

static let numeric: Date.FormatStyle.DateStyle

A date style with the month, day of month, and year components represented as numeric values.

static let omitted: Date.FormatStyle.DateStyle

A date style with no date-related components represented.

### Comparing Date Styles

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Specifying the Date Format

func day(Date.FormatStyle.Symbol.Day) -> Date.FormatStyle

Modifies the date format style to use the specified day format style.

func dayOfYear(Date.FormatStyle.Symbol.DayOfYear) -> Date.FormatStyle

Modifies the date format style to use the specified day of the year format style.

func era(Date.FormatStyle.Symbol.Era) -> Date.FormatStyle

Modifies the date format style to use the specified era format style.

func month(Date.FormatStyle.Symbol.Month) -> Date.FormatStyle

Modifies the date format style to use the specified month format style.

func quarter(Date.FormatStyle.Symbol.Quarter) -> Date.FormatStyle

Modifies the date format style to use the specified quarter format style.

func week(Date.FormatStyle.Symbol.Week) -> Date.FormatStyle

Modifies the date format style to use the specified week format style.

func weekday(Date.FormatStyle.Symbol.Weekday) -> Date.FormatStyle

Modifies the date format style to use the specified weekday format style.

func year(Date.FormatStyle.Symbol.Year) -> Date.FormatStyle

Modifies the date format style to use the specified year format style.

