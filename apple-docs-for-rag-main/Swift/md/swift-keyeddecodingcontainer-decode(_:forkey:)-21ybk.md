

- Swift
- KeyedDecodingContainer
-  decode(\_:forKey:) 

Instance Method

# decode(\_:forKey:)

Decodes a value of the given type for the given key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decode(
    _ type: UInt32.Type,
    forKey key: KeyedDecodingContainer.Key
) throws -> UInt32
```

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

