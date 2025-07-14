

- Swift
-  KeyedEncodingContainerProtocol 

Protocol

# KeyedEncodingContainerProtocol

A type that provides a view into an encoder’s storage and is used to hold the encoded properties of an encodable type in a keyed manner.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol KeyedEncodingContainerProtocol
```

## Overview

Encoders should provide types conforming to `KeyedEncodingContainerProtocol` for their format.

## Topics

### Associated Types

associatedtype Key : CodingKey

**Required**

### Instance Properties

var codingPath: [any CodingKey]

The path of coding keys taken to get to this point in encoding.

**Required**

### Instance Methods

func encode(Int16, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(UInt16, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(Float, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(UInt64, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(Bool, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(Int, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(Int128, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(String, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(UInt128, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(Int64, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(UInt, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(UInt8, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode&lt;T>(T, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(UInt32, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(Double, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(Int32, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encode(Int8, forKey: Self.Key) throws

Encodes the given value for the given key.

**Required** Default implementations provided.

func encodeConditional&lt;T>(T, forKey: Self.Key) throws

Encodes a reference to the given object only if it is encoded unconditionally elsewhere in the payload (previously, or in the future).

**Required** Default implementation provided.

func encodeIfPresent(UInt8?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(Float?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(Int8?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(UInt64?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(Bool?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(UInt128?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(UInt?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(Int?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(Int32?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(Int16?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent&lt;T>(T?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(String?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(Double?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(UInt16?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(UInt32?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(Int128?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeIfPresent(Int64?, forKey: Self.Key) throws

Encodes the given value for the given key if it is not `nil`.

**Required** Default implementations provided.

func encodeNil(forKey: Self.Key) throws

Encodes a null value for the given key.

**Required**

func nestedContainer&lt;NestedKey>(keyedBy: NestedKey.Type, forKey: Self.Key) -> KeyedEncodingContainer&lt;NestedKey>

Stores a keyed encoding container for the given key and returns it.

**Required**

func nestedUnkeyedContainer(forKey: Self.Key) -> any UnkeyedEncodingContainer

Stores an unkeyed encoding container for the given key and returns it.

**Required**

func superEncoder() -> any Encoder

Stores a new nested container for the default `super` key and returns a new encoder instance for encoding `super` into that container.

**Required**

func superEncoder(forKey: Self.Key) -> any Encoder

Stores a new nested container for the given key and returns a new encoder instance for encoding `super` into that container.

**Required**

## Relationships

### Conforming Types

- KeyedEncodingContainer

## See Also

### Encoding Containers

protocol SingleValueEncodingContainer

A container that can support the storage and direct encoding of a single non-keyed value.

struct KeyedEncodingContainer

A concrete container that provides a view into an encoder’s storage, making the encoded properties of an encodable type accessible by keys.

protocol UnkeyedEncodingContainer

A type that provides a view into an encoder’s storage and is used to hold the encoded properties of an encodable type sequentially, without keys.

