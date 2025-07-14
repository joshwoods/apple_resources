

- Swift
-  DecodingError 

Enumeration

# DecodingError

An error that occurs during the decoding of a value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum DecodingError
```

## Topics

### Structures

struct Context

The context in which the error occurred.

### Enumeration Cases

case dataCorrupted(DecodingError.Context)

An indication that the data is corrupted or otherwise invalid.

case keyNotFound(any CodingKey, DecodingError.Context)

An indication that a keyed decoding container was asked for an entry for the given key, but did not contain one.

case typeMismatch(any Any.Type, DecodingError.Context)

An indication that a value of the given type could not be decoded because it did not match the type of what was found in the encoded payload.

case valueNotFound(any Any.Type, DecodingError.Context)

An indication that a non-optional value of the given type was expected, but a null value was found.

### Type Methods

static func dataCorruptedError&lt;C>(forKey: C.Key, in: C, debugDescription: String) -> DecodingError

Returns a new `.dataCorrupted` error using a constructed coding path and the given debug description.

static func dataCorruptedError(in: any SingleValueDecodingContainer, debugDescription: String) -> DecodingError

Returns a new `.dataCorrupted` error using a constructed coding path and the given debug description.

static func dataCorruptedError(in: any UnkeyedDecodingContainer, debugDescription: String) -> DecodingError

Returns a new `.dataCorrupted` error using a constructed coding path and the given debug description.

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

enum EncodingError

An error that occurs during the encoding of a value.

