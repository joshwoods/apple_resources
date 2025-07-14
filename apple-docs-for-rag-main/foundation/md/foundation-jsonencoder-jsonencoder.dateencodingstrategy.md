

- Foundation
- JSONEncoder
-  JSONEncoder.DateEncodingStrategy 

Enumeration

# JSONEncoder.DateEncodingStrategy

The formatting strategies available for formatting dates when encoding a date as JSON.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum DateEncodingStrategy
```

## Topics

### Default Formats

case deferredToDate

The strategy that uses formatting from the Date structure.

### Standard Formats

case iso8601

The strategy that formats dates according to the ISO 8601 and RFC 3339 standards.

### Custom Formats

case formatted(DateFormatter)

The strategy that defers formatting settings to a supplied date formatter.

case custom((Date, any Encoder) throws -> Void)

The strategy that formats custom dates by calling a user-defined function.

### Epoch Formats

case millisecondsSince1970

The strategy that encodes dates in terms of milliseconds since midnight UTC on January 1, 1970.

case secondsSince1970

The strategy that encodes dates in terms of seconds since midnight UTC on January 1, 1970.

## Relationships

### Conforms To

- Sendable

## See Also

### Encoding Dates

var dateEncodingStrategy: JSONEncoder.DateEncodingStrategy

The strategy used when encoding dates as part of a JSON object.

