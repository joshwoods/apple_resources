

- Swift
-  EncodingError 

Enumeration

# EncodingError

An error that occurs during the encoding of a value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum EncodingError
```

## Topics

### Structures

struct Context

The context in which the error occurred.

### Enumeration Cases

case invalidValue(Any, EncodingError.Context)

An indication that an encoder or its containers could not encode the given value.

## Relationships

### Conforms To

- Copyable
- Error
- LocalizedError
- Sendable

## See Also

### Encoders and Decoders

protocol Encoder

A type that can encode values into a native format for external representation.

protocol Decoder

A type that can decode values from a native format into in-memory representations.

enum DecodingError

An error that occurs during the decoding of a value.

