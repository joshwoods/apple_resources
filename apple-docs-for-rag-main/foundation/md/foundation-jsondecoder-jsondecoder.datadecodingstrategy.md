

- Foundation
- JSONDecoder
-  JSONDecoder.DataDecodingStrategy 

Enumeration

# JSONDecoder.DataDecodingStrategy

The strategies for decoding raw data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum DataDecodingStrategy
```

## Topics

### Base64 Decoding

case base64

The strategy that decodes data using Base 64 decoding.

### Custom Decoding

case custom((any Decoder) throws -> Data)

The strategy that decodes data using a user-defined function.

### Data Decoding

case deferredToData

The strategy that encodes data using the encoding specified by the data instance itself.

## Relationships

### Conforms To

- Sendable

## See Also

### Decoding Raw Data

var dataDecodingStrategy: JSONDecoder.DataDecodingStrategy

The strategy that a decoder uses to decode raw data.

