

- Swift
-  KeyedEncodingContainer 

Structure

# KeyedEncodingContainer

A concrete container that provides a view into an encoder’s storage, making the encoded properties of an encodable type accessible by keys.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct KeyedEncodingContainer where K : CodingKey
```

## Topics

### Initializers

init&lt;Container>(Container)

Creates a new instance with the given container.

### Instance Properties

var codingPath: [any CodingKey]

The path of coding keys taken to get to this point in encoding.

### Instance Methods

func encode&lt;T, C>(CodableConfiguration&lt;T?, C>, forKey: KeyedEncodingContainer&lt;K>.Key) throws

func encode(UInt, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode&lt;T>(T, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(UInt8, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(Int64, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(String, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(Int, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(Int128, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(UInt64, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(Int32, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(Int16, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(UInt16, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(UInt128, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(Float, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(UInt32, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(Int8, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(Double, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode(Bool, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key.

func encode&lt;T, C>(T, forKey: KeyedEncodingContainer&lt;K>.Key, configuration: C.Type) throws

func encode&lt;T>(T, forKey: KeyedEncodingContainer&lt;K>.Key, configuration: T.EncodingConfiguration) throws

func encodeConditional&lt;T>(T, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes a reference to the given object only if it is encoded unconditionally elsewhere in the payload (previously, or in the future).

func encodeIfPresent(Int?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int16?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(String?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt16?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt32?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent&lt;T>(T?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Float?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int32?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int64?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt128?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Bool?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int128?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt64?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Int8?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(UInt8?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent(Double?, forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes the given value for the given key if it is not `nil`.

func encodeIfPresent&lt;T>(T?, forKey: KeyedEncodingContainer&lt;K>.Key, configuration: T.EncodingConfiguration) throws

func encodeIfPresent&lt;T, C>(T?, forKey: KeyedEncodingContainer&lt;K>.Key, configuration: C.Type) throws

func encodeNil(forKey: KeyedEncodingContainer&lt;K>.Key) throws

Encodes a null value for the given key.

func encodePredicateExpression&lt;T, each Input>(T, forKey: KeyedEncodingContainer&lt;K>.Key, variable: repeat PredicateExpressions.Variable&lt;each Input>, predicateConfiguration: PredicateCodableConfiguration) throws

func encodePredicateExpression&lt;T, each Input>(T, forKey: KeyedEncodingContainer&lt;K>.Key, variable: repeat PredicateExpressions.Variable&lt;each Input>, predicateConfiguration: PredicateCodableConfiguration) throws

func encodePredicateExpressionIfPresent&lt;T, each Input>(T?, forKey: KeyedEncodingContainer&lt;K>.Key, variable: repeat PredicateExpressions.Variable&lt;each Input>, predicateConfiguration: PredicateCodableConfiguration) throws

func encodePredicateExpressionIfPresent&lt;T, each Input>(T?, forKey: KeyedEncodingContainer&lt;K>.Key, variable: repeat PredicateExpressions.Variable&lt;each Input>, predicateConfiguration: PredicateCodableConfiguration) throws

func nestedContainer&lt;NestedKey>(keyedBy: NestedKey.Type, forKey: KeyedEncodingContainer&lt;K>.Key) -> KeyedEncodingContainer&lt;NestedKey>

Stores a keyed encoding container for the given key and returns it.

func nestedUnkeyedContainer(forKey: KeyedEncodingContainer&lt;K>.Key) -> any UnkeyedEncodingContainer

Stores an unkeyed encoding container for the given key and returns it.

func superEncoder() -> any Encoder

Stores a new nested container for the default `super` key and returns a new encoder instance for encoding `super` into that container.

func superEncoder(forKey: KeyedEncodingContainer&lt;K>.Key) -> any Encoder

Stores a new nested container for the given key and returns a new encoder instance for encoding `super` into that container.

### Type Aliases

typealias Key

### Default Implementations

KeyedEncodingContainerProtocol Implementations

## Relationships

### Conforms To

- KeyedEncodingContainerProtocol

## See Also

### Encoding Containers

protocol SingleValueEncodingContainer

A container that can support the storage and direct encoding of a single non-keyed value.

protocol KeyedEncodingContainerProtocol

A type that provides a view into an encoder’s storage and is used to hold the encoded properties of an encodable type in a keyed manner.

protocol UnkeyedEncodingContainer

A type that provides a view into an encoder’s storage and is used to hold the encoded properties of an encodable type sequentially, without keys.

