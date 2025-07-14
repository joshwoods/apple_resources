

- Foundation
- Date
-  Date.ParseStrategy 

Structure

# Date.ParseStrategy

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ParseStrategy
```

## Topics

### Initializers

init(format: Date.FormatString, locale: Locale?, timeZone: TimeZone, calendar: Calendar, isLenient: Bool, twoDigitStartDate: Date)

### Instance Properties

var calendar: Calendar

var format: String

var isLenient: Bool

var locale: Locale?

var timeZone: TimeZone

var twoDigitStartDate: Date

### Default Implementations

ParseStrategy Implementations

## Relationships

### Conforms To

- Copyable
- CustomConsumingRegexComponent
- Decodable
- Encodable
- Equatable
- Hashable
- ParseStrategy
- RegexComponent
- Sendable

