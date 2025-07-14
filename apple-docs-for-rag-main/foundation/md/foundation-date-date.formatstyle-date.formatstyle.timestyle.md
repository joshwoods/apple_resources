

- Foundation
- Date
- Date.FormatStyle
-  Date.FormatStyle.TimeStyle 

Structure

# Date.FormatStyle.TimeStyle

Type that defines time styles varied in length or components included.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct TimeStyle
```

## Overview

The exact format depends on the locale. Possible time styles include omitted, shortened, standard, and complete.

The following code sample shows a variety of time style format results using the `en_US` locale.

```
let meetingDate = Date()
meetingDate.formatted(date: .numeric, time: .omitted)
// 10/17/2020

meetingDate.formatted(date: .numeric, time: .shortened)
// 10/17/2020, 9:54 PM

meetingDate.formatted(date: .numeric, time: .standard)
// 10/17/2020, 9:54:29 PM

meetingDate.formatted(date: .numeric, time: .complete)
// 10/17/2020, 9:54:29 PM CDT

meetingDate.formatted()
// 10/17/2020, 9:54 PM

```

The default time style is shortened.

## Topics

### Modifying a Time Style

static let complete: Date.FormatStyle.TimeStyle

A time style with all components represented.

static let omitted: Date.FormatStyle.TimeStyle

A time style with no time-related components represented.

static let shortened: Date.FormatStyle.TimeStyle

A shortened time style with only the hour, minute, and day period components represented.

static let standard: Date.FormatStyle.TimeStyle

A time style with all components except the time zone represented.

### Comparing Time Styles

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

### Specifying the Time Format

func hour(Date.FormatStyle.Symbol.Hour) -> Date.FormatStyle

Modifies the date format style to use the specified hour format style.

func minute(Date.FormatStyle.Symbol.Minute) -> Date.FormatStyle

Modifies the date format style to use the specified minute format style.

func second(Date.FormatStyle.Symbol.Second) -> Date.FormatStyle

Modifies the date format style to use the specified second format style.

func secondFraction(Date.FormatStyle.Symbol.SecondFraction) -> Date.FormatStyle

Modifies the date format style to use the specified second fraction format style.

func timeZone(Date.FormatStyle.Symbol.TimeZone) -> Date.FormatStyle

Modifies the date format style to use the specified time zone format style.

