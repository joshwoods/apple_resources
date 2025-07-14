

- Swift
- UnkeyedDecodingContainer
-  decodeIfPresent(\_:) 

Instance Method

# decodeIfPresent(\_:)

Decodes a value of the given type, if present.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func decodeIfPresent(_ type: Double.Type) throws -> Double?
```

**Required** Default implementations provided.

## Parameters 

`type`  

The type of value to decode.

## Return Value

A decoded value of the requested type, or `nil` if the value is a null value, or if there are no more elements to decode.

## Discussion

This method returns `nil` if the container has no elements left to decode, or if the value is null. The difference between these states can be distinguished by checking `isAtEnd`.

Throws

`DecodingError.typeMismatch` if the encountered encoded value is not convertible to the requested type.

## Default Implementations

### UnkeyedDecodingContainer Implementations

func decodeIfPresent(Int128.Type) throws -> Int128?

Decodes a value of the given type, if present.

func decodeIfPresent(UInt16.Type) throws -> UInt16?

Decodes a value of the given type, if present.

func decodeIfPresent(UInt.Type) throws -> UInt?

Decodes a value of the given type, if present.

func decodeIfPresent(Float.Type) throws -> Float?

Decodes a value of the given type, if present.

func decodeIfPresent(UInt8.Type) throws -> UInt8?

Decodes a value of the given type, if present.

func decodeIfPresent(Int8.Type) throws -> Int8?

Decodes a value of the given type, if present.

func decodeIfPresent(UInt128.Type) throws -> UInt128?

Decodes a value of the given type, if present.

func decodeIfPresent(UInt32.Type) throws -> UInt32?

Decodes a value of the given type, if present.

func decodeIfPresent&lt;T>(T.Type) throws -> T?

Decodes a value of the given type, if present.

func decodeIfPresent(UInt64.Type) throws -> UInt64?

Decodes a value of the given type, if present.

func decodeIfPresent(Double.Type) throws -> Double?

Decodes a value of the given type, if present.

func decodeIfPresent(String.Type) throws -> String?

Decodes a value of the given type, if present.

func decodeIfPresent(Int32.Type) throws -> Int32?

Decodes a value of the given type, if present.

func decodeIfPresent(Bool.Type) throws -> Bool?

Decodes a value of the given type, if present.

func decodeIfPresent(Int16.Type) throws -> Int16?

Decodes a value of the given type, if present.

func decodeIfPresent(Int.Type) throws -> Int?

Decodes a value of the given type, if present.

func decodeIfPresent(Int64.Type) throws -> Int64?

Decodes a value of the given type, if present.

