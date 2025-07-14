

- Foundation
- JSONEncoder
-  JSONEncoder.DataEncodingStrategy 

Enumeration

# JSONEncoder.DataEncodingStrategy

The strategies for encoding raw data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum DataEncodingStrategy
```

## Topics

### Base64 Encoding

case base64

The strategy that encodes data using Base 64 encoding.

### Custom Encoding

case custom((Data, any Encoder) throws -> Void)

The strategy that encodes data using a user-defined function.

### Data Encoding

case deferredToData

The strategy that encodes data using the encoding specified by the data instance itself.

## Relationships

### Conforms To

- Sendable

## See Also

### Encoding Raw Data

var dataEncodingStrategy: JSONEncoder.DataEncodingStrategy

The strategy that an encoder uses to encode raw data.

