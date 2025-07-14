

- Swift
-  Encoder 

Protocol

# Encoder

A type that can encode values into a native format for external representation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol Encoder
```

## Topics

### Instance Properties

var codingPath: [any CodingKey]

The path of coding keys taken to get to this point in encoding.

**Required**

var userInfo: [CodingUserInfoKey : Any]

Any contextual information set by the user for encoding.

**Required**

### Instance Methods

func container&lt;Key>(keyedBy: Key.Type) -> KeyedEncodingContainer&lt;Key>

Returns an encoding container appropriate for holding multiple values keyed by the given key type.

**Required**

func singleValueContainer() -> any SingleValueEncodingContainer

Returns an encoding container appropriate for holding a single primitive value.

**Required**

func unkeyedContainer() -> any UnkeyedEncodingContainer

Returns an encoding container appropriate for holding multiple unkeyed values.

**Required**

## See Also

### Encoders and Decoders

protocol Decoder

A type that can decode values from a native format into in-memory representations.

enum EncodingError

An error that occurs during the encoding of a value.

enum DecodingError

An error that occurs during the decoding of a value.

