

- Swift
-  UnkeyedEncodingContainer 

Protocol

# UnkeyedEncodingContainer

A type that provides a view into an encoder’s storage and is used to hold the encoded properties of an encodable type sequentially, without keys.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol UnkeyedEncodingContainer
```

## Overview

Encoders should provide types conforming to `UnkeyedEncodingContainer` for their format.

## Topics

### Instance Properties

var codingPath: [any CodingKey]

The path of coding keys taken to get to this point in encoding.

**Required**

var count: Int

The number of elements encoded into the container.

**Required**

### Instance Methods

func encode(Float) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(Double) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(Bool) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(Int) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(UInt) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(UInt128) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(UInt8) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(Int64) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(UInt16) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(String) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(Int128) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(UInt32) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(Int8) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(Int16) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(Int32) throws

Encodes the given value.

**Required** Default implementations provided.

func encode&lt;T>(T) throws

Encodes the given value.

**Required** Default implementations provided.

func encode(UInt64) throws

Encodes the given value.

**Required** Default implementations provided.

func encode&lt;T, C>(T, configuration: C.Type) throws

func encode&lt;T>(T, configuration: T.EncodingConfiguration) throws

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encode&lt;T>(contentsOf: T) throws

Encodes the elements of the given sequence.

**Required** Default implementations provided.

func encodeConditional&lt;T>(T) throws

Encodes a reference to the given object only if it is encoded unconditionally elsewhere in the payload (previously, or in the future).

**Required** Default implementation provided.

func encodeNil() throws

Encodes a null value.

**Required**

func encodePredicateExpression&lt;T, each Input>(T, variable: repeat PredicateExpressions.Variable&lt;each Input>, predicateConfiguration: PredicateCodableConfiguration) throws

func encodePredicateExpression&lt;T, each Input>(T, variable: repeat PredicateExpressions.Variable&lt;each Input>, predicateConfiguration: PredicateCodableConfiguration) throws

func encodePredicateExpressionIfPresent&lt;T, each Input>(T?, variable: repeat PredicateExpressions.Variable&lt;each Input>, predicateConfiguration: PredicateCodableConfiguration) throws

func encodePredicateExpressionIfPresent&lt;T, each Input>(T?, variable: repeat PredicateExpressions.Variable&lt;each Input>, predicateConfiguration: PredicateCodableConfiguration) throws

func nestedContainer&lt;NestedKey>(keyedBy: NestedKey.Type) -> KeyedEncodingContainer&lt;NestedKey>

Encodes a nested container keyed by the given type and returns it.

**Required**

func nestedUnkeyedContainer() -> any UnkeyedEncodingContainer

Encodes an unkeyed encoding container and returns it.

**Required**

func superEncoder() -> any Encoder

Encodes a nested container and returns an `Encoder` instance for encoding `super` into that container.

**Required**

## See Also

### Encoding Containers

protocol SingleValueEncodingContainer

A container that can support the storage and direct encoding of a single non-keyed value.

struct KeyedEncodingContainer

A concrete container that provides a view into an encoder’s storage, making the encoded properties of an encodable type accessible by keys.

protocol KeyedEncodingContainerProtocol

A type that provides a view into an encoder’s storage and is used to hold the encoded properties of an encodable type in a keyed manner.

