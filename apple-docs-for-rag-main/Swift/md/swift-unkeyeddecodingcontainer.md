

- Swift
-  UnkeyedDecodingContainer 

Protocol

# UnkeyedDecodingContainer

A type that provides a view into a decoder’s storage and is used to hold the encoded properties of a decodable type sequentially, without keys.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol UnkeyedDecodingContainer
```

## Overview

Decoders should provide types conforming to `UnkeyedDecodingContainer` for their format.

## Topics

### Instance Properties

var codingPath: [any CodingKey]

The path of coding keys taken to get to this point in decoding.

**Required**

var count: Int?

The number of elements contained within this container.

**Required**

var currentIndex: Int

The current decoding index of the container (i.e. the index of the next element to be decoded.) Incremented after every successful decode call.

**Required**

var isAtEnd: Bool

A Boolean value indicating whether there are no more elements left to be decoded in the container.

**Required**

### Instance Methods

func decode(UInt64.Type) throws -> UInt64

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(Double.Type) throws -> Double

Decodes a value of the given type.

**Required** Default implementations provided.

func decode&lt;T>(T.Type) throws -> T

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(UInt32.Type) throws -> UInt32

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(UInt16.Type) throws -> UInt16

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(String.Type) throws -> String

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(Int32.Type) throws -> Int32

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(Int16.Type) throws -> Int16

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(UInt128.Type) throws -> UInt128

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(Int64.Type) throws -> Int64

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(UInt.Type) throws -> UInt

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(Bool.Type) throws -> Bool

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(Int.Type) throws -> Int

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(Int128.Type) throws -> Int128

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(Float.Type) throws -> Float

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(Int8.Type) throws -> Int8

Decodes a value of the given type.

**Required** Default implementations provided.

func decode(UInt8.Type) throws -> UInt8

Decodes a value of the given type.

**Required** Default implementations provided.

func decode&lt;T>(T.Type, configuration: T.DecodingConfiguration) throws -> T

func decode&lt;T, C>(T.Type, configuration: C.Type) throws -> T

func decodeIfPresent(Float.Type) throws -> Float?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(UInt32.Type) throws -> UInt32?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(Int16.Type) throws -> Int16?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(Int.Type) throws -> Int?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(UInt.Type) throws -> UInt?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(UInt8.Type) throws -> UInt8?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(Int8.Type) throws -> Int8?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(Int64.Type) throws -> Int64?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(UInt16.Type) throws -> UInt16?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(Int32.Type) throws -> Int32?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(UInt128.Type) throws -> UInt128?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(Double.Type) throws -> Double?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(UInt64.Type) throws -> UInt64?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(String.Type) throws -> String?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(Bool.Type) throws -> Bool?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent(Int128.Type) throws -> Int128?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent&lt;T>(T.Type) throws -> T?

Decodes a value of the given type, if present.

**Required** Default implementations provided.

func decodeIfPresent&lt;T, C>(T.Type, configuration: C.Type) throws -> T?

func decodeIfPresent&lt;T>(T.Type, configuration: T.DecodingConfiguration) throws -> T?

func decodeNil() throws -> Bool

Decodes a null value.

**Required**

func decodePredicateExpression&lt;each Input, Output>(input: repeat (each Input).Type, output: Output.Type, predicateConfiguration: PredicateCodableConfiguration) throws -> (expression: any PredicateExpression&lt;Output>, variable: (repeat PredicateExpressions.Variable&lt;each Input>))

func decodePredicateExpression&lt;each Input>(input: repeat (each Input).Type, predicateConfiguration: PredicateCodableConfiguration) throws -> (expression: any PredicateExpression&lt;Bool>, variable: (repeat PredicateExpressions.Variable&lt;each Input>))

func decodePredicateExpressionIfPresent&lt;each Input, Output>(input: repeat (each Input).Type, output: Output.Type, predicateConfiguration: PredicateCodableConfiguration) throws -> (expression: any PredicateExpression&lt;Output>, variable: (repeat PredicateExpressions.Variable&lt;each Input>))?

func decodePredicateExpressionIfPresent&lt;each Input>(input: repeat (each Input).Type, predicateConfiguration: PredicateCodableConfiguration) throws -> (expression: any PredicateExpression&lt;Bool>, variable: (repeat PredicateExpressions.Variable&lt;each Input>))?

func nestedContainer&lt;NestedKey>(keyedBy: NestedKey.Type) throws -> KeyedDecodingContainer&lt;NestedKey>

Decodes a nested container keyed by the given type.

**Required**

func nestedUnkeyedContainer() throws -> any UnkeyedDecodingContainer

Decodes an unkeyed nested container.

**Required**

func superDecoder() throws -> any Decoder

Decodes a nested container and returns a `Decoder` instance for decoding `super` from that container.

**Required**

## See Also

### Decoding Containers

struct KeyedDecodingContainer

A concrete container that provides a view into a decoder’s storage, making the encoded properties of a decodable type accessible by keys.

protocol SingleValueDecodingContainer

A container that can support the storage and direct decoding of a single nonkeyed value.

protocol KeyedDecodingContainerProtocol

A type that provides a view into a decoder’s storage and is used to hold the encoded properties of a decodable type in a keyed manner.

