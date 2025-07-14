

- Swift
-  Decoder 

Protocol

# Decoder

A type that can decode values from a native format into in-memory representations.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol Decoder
```

## Topics

### Instance Properties

var codingPath: [any CodingKey]

The path of coding keys taken to get to this point in decoding.

**Required**

var userInfo: [CodingUserInfoKey : Any]

Any contextual information set by the user for decoding.

**Required**

### Instance Methods

func container&lt;Key>(keyedBy: Key.Type) throws -> KeyedDecodingContainer&lt;Key>

Returns the data stored in this decoder as represented in a container keyed by the given key type.

**Required**

func singleValueContainer() throws -> any SingleValueDecodingContainer

Returns the data stored in this decoder as represented in a container appropriate for holding a single primitive value.

**Required**

func unkeyedContainer() throws -> any UnkeyedDecodingContainer

Returns the data stored in this decoder as represented in a container appropriate for holding values with no keys.

**Required**

## See Also

### Encoders and Decoders

protocol Encoder

A type that can encode values into a native format for external representation.

enum EncodingError

An error that occurs during the encoding of a value.

enum DecodingError

An error that occurs during the decoding of a value.

