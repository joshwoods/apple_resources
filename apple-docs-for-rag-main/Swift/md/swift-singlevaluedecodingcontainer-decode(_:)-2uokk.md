

- Swift
- SingleValueDecodingContainer
-  decode(\_:) 

Instance Method

# decode(\_:)

Decodes a single value of the given type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decode(_ type: UInt64.Type) throws -> UInt64
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

func decode(UInt128.Type) throws -> UInt128

Decodes a single value of the given type.

func decode(UInt128.Type) throws -> UInt128

Decodes a single value of the given type.

func decode(Int128.Type) throws -> Int128

Decodes a single value of the given type.

func decode(Int128.Type) throws -> Int128

Decodes a single value of the given type.

