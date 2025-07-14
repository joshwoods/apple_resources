

- Foundation
- Date
- Date.ISO8601FormatStyle
-  Date.ISO8601FormatStyle.DateTimeSeparator 

Enumeration

# Date.ISO8601FormatStyle.DateTimeSeparator

Type describing the character separating the date and time components of a date in an ISO 8601 date format.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum DateTimeSeparator
```

## Topics

### Specifying ISO 8601 Format Style Date Time Separators

case space

Specifies a space character separating date and time components in an ISO 8601 date format style.

case standard

Specifies no separator between the date and time components in an ISO 8601 date format style.

### Comparing ISO 8601 Format Style Date Time Separators

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

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

### Supporting Types

enum DateSeparator

A type describing the character separating year, month, and day components of a date in an ISO 8601 date format.

enum TimeSeparator

Type describing the character separating the time components of a date in an ISO 8601 date format.

enum TimeZoneSeparator

A type describing the character separating the time and time zone of a date in an ISO 8601 date format.

