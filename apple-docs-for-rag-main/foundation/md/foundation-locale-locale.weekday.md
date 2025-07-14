

- Foundation
- Locale
-  Locale.Weekday 

Enumeration

# Locale.Weekday

A type that represents weekdays, used for indicating a locale’s first day of the week.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Weekday
```

## Topics

### Using defined weekdays

case monday

The weekday enumeration value for Monday.

case tuesday

The weekday enumeration value for Tuesday.

case wednesday

The weekday enumeration value for Wednesday.

case thursday

The weekday enumeration value for Thursday.

case friday

The weekday enumeration value for Friday.

case saturday

The weekday enumeration value for Saturday.

case sunday

The weekday enumeration value for Sunday.

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

var hourCycle: Locale.HourCycle

The hour cycle used by the locale, like one-to-twelve or zero-to-twenty-three.

enum HourCycle

A type that represents the hour cycle used in a locale, like one-to-twelve or zero-to-twenty-three.

var timeZone: TimeZone?

The time zone associated with the locale, if any.

