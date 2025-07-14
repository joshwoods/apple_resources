

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.VerbatimHour
-  Date.FormatStyle.Symbol.VerbatimHour.Clock 

Structure

# Date.FormatStyle.Symbol.VerbatimHour.Clock

A type that specifies a clock representation for the format of an hour.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Clock
```

## Topics

### Modifying a Verbatim Hour Clock

static let twelveHour: Date.FormatStyle.Symbol.VerbatimHour.Clock

A clock that portrays the hour using a 12-hour clock.

static let twentyFourHour: Date.FormatStyle.Symbol.VerbatimHour.Clock

A clock that portrays the hour using a 24-hour clock.

### Comparing Verbatim Hour Clocks

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

### Supporting Structures

struct HourCycle

A type that specifies the start of a clock representation for the format of a hour.

