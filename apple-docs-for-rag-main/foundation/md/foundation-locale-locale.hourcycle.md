

- Foundation
- Locale
-  Locale.HourCycle 

Enumeration

# Locale.HourCycle

A type that represents the hour cycle used in a locale, like one-to-twelve or zero-to-twenty-three.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum HourCycle
```

## Topics

### Using defined hour cycles

case zeroToEleven

A twelve hour cycle, counted from 0 to 11.

case oneToTwelve

A twelve hour cycle, counted from 1 to 12.

case zeroToTwentyThree

A twenty-four hour cycle, counted from 0 to 23.

case oneToTwentyFour

A twenty-four hour cycle, counted from 1 to 24.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting date and time components

var firstDayOfWeek: Locale.Weekday

The first day of the week as represented by this locale.

enum Weekday

A type that represents weekdays, used for indicating a locale’s first day of the week.

var hourCycle: Locale.HourCycle

The hour cycle used by the locale, like one-to-twelve or zero-to-twenty-three.

var timeZone: TimeZone?

The time zone associated with the locale, if any.

