

- Swift
- KeyedDecodingContainerProtocol
-  decode(\_:forKey:) 

Instance Method

# decode(\_:forKey:)

Decodes a value of the given type for the given key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decode(
    _ type: Int8.Type,
    forKey key: Self.Key
) throws -> Int8
```

**Required** Default implementations provided.

## Parameters 

`type`  

The type of value to decode.

`key`  

The key that the decoded value is associated with.

## Return Value

A value of the requested type, if present for the given key and convertible to the requested type.

## Discussion

Throws

`DecodingError.typeMismatch` if the encountered encoded value is not convertible to the requested type.

Throws

`DecodingError.keyNotFound` if `self` does not have an entry for the given key.

Throws

`DecodingError.valueNotFound` if `self` has a null entry for the given key.

## Default Implementations

### KeyedDecodingContainerProtocol Implementations

func decode(Int128.Type, forKey: Self.Key) throws -> Int128

Decodes a value of the given type for the given key.

func decode(UInt128.Type, forKey: Self.Key) throws -> UInt128

Decodes a value of the given type for the given key.

