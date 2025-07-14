

- Swift
-  KeyedDecodingContainerProtocol 

Protocol

# KeyedDecodingContainerProtocol

A type that provides a view into a decoder’s storage and is used to hold the encoded properties of a decodable type in a keyed manner.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol KeyedDecodingContainerProtocol
```

## Overview

Decoders should provide types conforming to `UnkeyedDecodingContainer` for their format.

## Topics

### Associated Types

associatedtype Key : CodingKey

**Required**

### Instance Properties

var allKeys: [Self.Key]

All the keys the `Decoder` has for this container.

**Required**

var codingPath: [any CodingKey]

The path of coding keys taken to get to this point in decoding.

**Required**

### Instance Methods

func contains(Self.Key) -> Bool

Returns a Boolean value indicating whether the decoder contains a value associated with the given key.

**Required**

func decode(UInt8.Type, forKey: Self.Key) throws -> UInt8

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(Int128.Type, forKey: Self.Key) throws -> Int128

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(UInt32.Type, forKey: Self.Key) throws -> UInt32

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(UInt.Type, forKey: Self.Key) throws -> UInt

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(Bool.Type, forKey: Self.Key) throws -> Bool

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(UInt128.Type, forKey: Self.Key) throws -> UInt128

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(Int16.Type, forKey: Self.Key) throws -> Int16

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(Int32.Type, forKey: Self.Key) throws -> Int32

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(UInt64.Type, forKey: Self.Key) throws -> UInt64

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(Int.Type, forKey: Self.Key) throws -> Int

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(Int64.Type, forKey: Self.Key) throws -> Int64

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(String.Type, forKey: Self.Key) throws -> String

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(UInt16.Type, forKey: Self.Key) throws -> UInt16

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(Int8.Type, forKey: Self.Key) throws -> Int8

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(Float.Type, forKey: Self.Key) throws -> Float

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode(Double.Type, forKey: Self.Key) throws -> Double

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decode&lt;T>(T.Type, forKey: Self.Key) throws -> T

Decodes a value of the given type for the given key.

**Required** Default implementations provided.

func decodeIfPresent(String.Type, forKey: Self.Key) throws -> String?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(Int64.Type, forKey: Self.Key) throws -> Int64?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(Double.Type, forKey: Self.Key) throws -> Double?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(UInt16.Type, forKey: Self.Key) throws -> UInt16?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(Bool.Type, forKey: Self.Key) throws -> Bool?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(Int32.Type, forKey: Self.Key) throws -> Int32?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(UInt32.Type, forKey: Self.Key) throws -> UInt32?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(UInt64.Type, forKey: Self.Key) throws -> UInt64?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(UInt8.Type, forKey: Self.Key) throws -> UInt8?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent&lt;T>(T.Type, forKey: Self.Key) throws -> T?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(UInt128.Type, forKey: Self.Key) throws -> UInt128?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(Int128.Type, forKey: Self.Key) throws -> Int128?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(Int16.Type, forKey: Self.Key) throws -> Int16?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(Int.Type, forKey: Self.Key) throws -> Int?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(Int8.Type, forKey: Self.Key) throws -> Int8?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(Float.Type, forKey: Self.Key) throws -> Float?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeIfPresent(UInt.Type, forKey: Self.Key) throws -> UInt?

Decodes a value of the given type for the given key, if present.

**Required** Default implementations provided.

func decodeNil(forKey: Self.Key) throws -> Bool

Decodes a null value for the given key.

**Required**

func nestedContainer&lt;NestedKey>(keyedBy: NestedKey.Type, forKey: Self.Key) throws -> KeyedDecodingContainer&lt;NestedKey>

Returns the data stored for the given key as represented in a container keyed by the given key type.

**Required**

func nestedUnkeyedContainer(forKey: Self.Key) throws -> any UnkeyedDecodingContainer

Returns the data stored for the given key as represented in an unkeyed container.

**Required**

func superDecoder() throws -> any Decoder

Returns a `Decoder` instance for decoding `super` from the container associated with the default `super` key.

**Required**

func superDecoder(forKey: Self.Key) throws -> any Decoder

Returns a `Decoder` instance for decoding `super` from the container associated with the given key.

**Required**

## Relationships

### Conforming Types

- KeyedDecodingContainer

## See Also

### Decoding Containers

struct KeyedDecodingContainer

A concrete container that provides a view into a decoder’s storage, making the encoded properties of a decodable type accessible by keys.

protocol SingleValueDecodingContainer

A container that can support the storage and direct decoding of a single nonkeyed value.

protocol UnkeyedDecodingContainer

A type that provides a view into a decoder’s storage and is used to hold the encoded properties of a decodable type sequentially, without keys.

