

- Swift
-  SingleValueEncodingContainer 

Protocol

# SingleValueEncodingContainer

A container that can support the storage and direct encoding of a single non-keyed value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol SingleValueEncodingContainer
```

## Topics

### Instance Properties

var codingPath: [any CodingKey]

The path of coding keys taken to get to this point in encoding.

**Required**

### Instance Methods

func encode(Int) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(Double) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(Float) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(Bool) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(UInt64) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(String) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(Int8) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(Int64) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(Int16) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(UInt128) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(UInt16) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode&lt;T>(T) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(UInt32) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(Int128) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(Int32) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(UInt) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encode(UInt8) throws

Encodes a single value of the given type.

**Required** Default implementations provided.

func encodeNil() throws

Encodes a null value.

**Required**

## See Also

### Encoding Containers

struct KeyedEncodingContainer

A concrete container that provides a view into an encoder’s storage, making the encoded properties of an encodable type accessible by keys.

protocol KeyedEncodingContainerProtocol

A type that provides a view into an encoder’s storage and is used to hold the encoded properties of an encodable type in a keyed manner.

protocol UnkeyedEncodingContainer

A type that provides a view into an encoder’s storage and is used to hold the encoded properties of an encodable type sequentially, without keys.

