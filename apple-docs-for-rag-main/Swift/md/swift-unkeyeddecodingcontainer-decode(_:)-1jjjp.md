

- Swift
- UnkeyedDecodingContainer
-  decode(\_:) 

Instance Method

# decode(\_:)

Decodes a value of the given type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func decode(_ type: UInt64.Type) throws -> UInt64
```

**Required** Default implementations provided.

## Parameters 

`type`  

The type of value to decode.

## Return Value

A value of the requested type, if present for the given key and convertible to the requested type.

## Discussion

Throws

`DecodingError.typeMismatch` if the encountered encoded value is not convertible to the requested type.

Throws

`DecodingError.valueNotFound` if the encountered encoded value is null, or of there are no more values to decode.

## Default Implementations

### UnkeyedDecodingContainer Implementations

func decode(UInt128.Type) throws -> UInt128

Decodes a value of the given type.

func decode(Int128.Type) throws -> Int128

Decodes a value of the given type.

