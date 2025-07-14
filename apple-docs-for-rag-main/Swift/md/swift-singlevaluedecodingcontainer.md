

- Swift
-  SingleValueDecodingContainer 

Protocol

# SingleValueDecodingContainer

A container that can support the storage and direct decoding of a single nonkeyed value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol SingleValueDecodingContainer
```

## Topics

### Instance Properties

var codingPath: [any CodingKey]

The path of coding keys taken to get to this point in encoding.

**Required**

### Instance Methods

func decode(UInt128.Type) throws -> UInt128

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(Int16.Type) throws -> Int16

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(Int128.Type) throws -> Int128

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(UInt64.Type) throws -> UInt64

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(Int8.Type) throws -> Int8

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode&lt;T>(T.Type) throws -> T

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(Bool.Type) throws -> Bool

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(Int.Type) throws -> Int

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(UInt.Type) throws -> UInt

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(Int64.Type) throws -> Int64

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(UInt8.Type) throws -> UInt8

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(Int32.Type) throws -> Int32

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(String.Type) throws -> String

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(UInt32.Type) throws -> UInt32

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(Double.Type) throws -> Double

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(UInt16.Type) throws -> UInt16

Decodes a single value of the given type.

**Required** Default implementations provided.

func decode(Float.Type) throws -> Float

Decodes a single value of the given type.

**Required** Default implementations provided.

func decodeNil() -> Bool

Decodes a null value.

**Required**

## See Also

### Decoding Containers

struct KeyedDecodingContainer

A concrete container that provides a view into a decoder’s storage, making the encoded properties of a decodable type accessible by keys.

protocol KeyedDecodingContainerProtocol

A type that provides a view into a decoder’s storage and is used to hold the encoded properties of a decodable type in a keyed manner.

protocol UnkeyedDecodingContainer

A type that provides a view into a decoder’s storage and is used to hold the encoded properties of a decodable type sequentially, without keys.

