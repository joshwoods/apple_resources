

- Swift
-  KeyedDecodingContainer 

Structure

# KeyedDecodingContainer

A concrete container that provides a view into a decoder’s storage, making the encoded properties of a decodable type accessible by keys.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct KeyedDecodingContainer where K : CodingKey
```

## Topics

### Initializers

init&lt;Container>(Container)

Creates a new instance with the given container.

### Instance Properties

var allKeys: [KeyedDecodingContainer&lt;K>.Key]

All the keys the decoder has for this container.

var codingPath: [any CodingKey]

The path of coding keys taken to get to this point in decoding.

### Instance Methods

func contains(KeyedDecodingContainer&lt;K>.Key) -> Bool

Returns a Boolean value indicating whether the decoder contains a value associated with the given key.

func decode(Int32.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Int32

Decodes a value of the given type for the given key.

func decode(Int8.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Int8

Decodes a value of the given type for the given key.

func decode&lt;T>(T.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> T

Decodes a value of the given type for the given key.

func decode(UInt32.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> UInt32

Decodes a value of the given type for the given key.

func decode(Float.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Float

Decodes a value of the given type for the given key.

func decode(String.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> String

Decodes a value of the given type for the given key.

func decode(Int128.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Int128

Decodes a value of the given type for the given key.

func decode(UInt.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> UInt

Decodes a value of the given type for the given key.

func decode(Int64.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Int64

Decodes a value of the given type for the given key.

func decode(UInt64.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> UInt64

Decodes a value of the given type for the given key.

func decode(Double.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Double

Decodes a value of the given type for the given key.

func decode(UInt128.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> UInt128

Decodes a value of the given type for the given key.

func decode(Int16.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Int16

Decodes a value of the given type for the given key.

func decode(Int.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Int

Decodes a value of the given type for the given key.

func decode(UInt8.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> UInt8

Decodes a value of the given type for the given key.

func decode&lt;T, C>(CodableConfiguration&lt;T?, C>.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> CodableConfiguration&lt;T?, C>

func decode(UInt16.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> UInt16

Decodes a value of the given type for the given key.

func decode(Bool.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Bool

Decodes a value of the given type for the given key.

func decode&lt;T>(T.Type, forKey: KeyedDecodingContainer&lt;K>.Key, configuration: T.DecodingConfiguration) throws -> T

func decode&lt;T, C>(T.Type, forKey: KeyedDecodingContainer&lt;K>.Key, configuration: C.Type) throws -> T

func decodeIfPresent(UInt8.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> UInt8?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Int8.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Int8?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Int64.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Int64?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Int.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Int?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent&lt;T>(T.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> T?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(UInt128.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> UInt128?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(UInt64.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> UInt64?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Float.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Float?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Int32.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Int32?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Bool.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Bool?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(String.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> String?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Double.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Double?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(UInt16.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> UInt16?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Int128.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Int128?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(UInt32.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> UInt32?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(Int16.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Int16?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent(UInt.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> UInt?

Decodes a value of the given type for the given key, if present.

func decodeIfPresent&lt;T>(T.Type, forKey: KeyedDecodingContainer&lt;K>.Key, configuration: T.DecodingConfiguration) throws -> T?

func decodeIfPresent&lt;T, C>(T.Type, forKey: KeyedDecodingContainer&lt;K>.Key, configuration: C.Type) throws -> T?

func decodeNil(forKey: KeyedDecodingContainer&lt;K>.Key) throws -> Bool

Decodes a null value for the given key.

func decodePredicateExpression&lt;each Input, Output>(forKey: KeyedDecodingContainer&lt;K>.Key, input: repeat (each Input).Type, output: Output.Type, predicateConfiguration: PredicateCodableConfiguration) throws -> (expression: any PredicateExpression&lt;Output>, variable: (repeat PredicateExpressions.Variable&lt;each Input>))

func decodePredicateExpression&lt;each Input>(forKey: KeyedDecodingContainer&lt;K>.Key, input: repeat (each Input).Type, predicateConfiguration: PredicateCodableConfiguration) throws -> (expression: any PredicateExpression&lt;Bool>, variable: (repeat PredicateExpressions.Variable&lt;each Input>))

func decodePredicateExpressionIfPresent&lt;each Input, Output>(forKey: KeyedDecodingContainer&lt;K>.Key, input: repeat (each Input).Type, output: Output.Type, predicateConfiguration: PredicateCodableConfiguration) throws -> (expression: any PredicateExpression&lt;Output>, variable: (repeat PredicateExpressions.Variable&lt;each Input>))?

func decodePredicateExpressionIfPresent&lt;each Input>(forKey: KeyedDecodingContainer&lt;K>.Key, input: repeat (each Input).Type, predicateConfiguration: PredicateCodableConfiguration) throws -> (expression: any PredicateExpression&lt;Bool>, variable: (repeat PredicateExpressions.Variable&lt;each Input>))?

func nestedContainer&lt;NestedKey>(keyedBy: NestedKey.Type, forKey: KeyedDecodingContainer&lt;K>.Key) throws -> KeyedDecodingContainer&lt;NestedKey>

Returns the data stored for the given key as represented in a container keyed by the given key type.

func nestedUnkeyedContainer(forKey: KeyedDecodingContainer&lt;K>.Key) throws -> any UnkeyedDecodingContainer

Returns the data stored for the given key as represented in an unkeyed container.

func superDecoder() throws -> any Decoder

Returns a `Decoder` instance for decoding `super` from the container associated with the default `super` key.

func superDecoder(forKey: KeyedDecodingContainer&lt;K>.Key) throws -> any Decoder

Returns a `Decoder` instance for decoding `super` from the container associated with the given key.

### Type Aliases

typealias Key

### Default Implementations

KeyedDecodingContainerProtocol Implementations

## Relationships

### Conforms To

- KeyedDecodingContainerProtocol

## See Also

### Decoding Containers

protocol SingleValueDecodingContainer

A container that can support the storage and direct decoding of a single nonkeyed value.

protocol KeyedDecodingContainerProtocol

A type that provides a view into a decoder’s storage and is used to hold the encoded properties of a decodable type in a keyed manner.

protocol UnkeyedDecodingContainer

A type that provides a view into a decoder’s storage and is used to hold the encoded properties of a decodable type sequentially, without keys.

