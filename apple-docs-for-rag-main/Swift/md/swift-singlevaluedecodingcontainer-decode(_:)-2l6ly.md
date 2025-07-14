

- Swift
- SingleValueDecodingContainer
-  decode(\_:) 

Instance Method

# decode(\_:)

Decodes a single value of the given type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func decode(_ type: Int128.Type) throws -> Int128
```

**Required** Default implementations provided.

## Parameters 

`type`  

The type to decode as.

## Return Value

A value of the requested type.

## Discussion

Throws

`DecodingError.typeMismatch` if the encountered encoded value cannot be converted to the requested type.

Throws

`DecodingError.valueNotFound` if the encountered encoded value is null.

## Default Implementations

### SingleValueDecodingContainer Implementations

func decode(Int128.Type) throws -> Int128

Decodes a single value of the given type.

func decode(UInt128.Type) throws -> UInt128

Decodes a single value of the given type.

func decode(UInt128.Type) throws -> UInt128

Decodes a single value of the given type.

func decode(Int128.Type) throws -> Int128

Decodes a single value of the given type.

