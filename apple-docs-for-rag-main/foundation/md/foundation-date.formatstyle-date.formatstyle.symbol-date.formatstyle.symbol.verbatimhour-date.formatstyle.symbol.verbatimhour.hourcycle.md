

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.VerbatimHour
-  Date.FormatStyle.Symbol.VerbatimHour.HourCycle 

Structure

# Date.FormatStyle.Symbol.VerbatimHour.HourCycle

A type that specifies the start of a clock representation for the format of a hour.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct HourCycle
```

## Topics

### Modifying a Verbatim Hour HourCycle

static let oneBased: Date.FormatStyle.Symbol.VerbatimHour.HourCycle

A hour cycle that indicates a clock that starts at one.

static let zeroBased: Date.FormatStyle.Symbol.VerbatimHour.HourCycle

A hour cycle that indicates a clock that starts at zero.

### Comparing Verbatim Hour Clock HourCycles

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

struct Clock

A type that specifies a clock representation for the format of an hour.

