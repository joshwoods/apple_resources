

- Swift
- KeyedDecodingContainer
-  decode(\_:forKey:) 

Instance Method

# decode(\_:forKey:)

Decodes a value of the given type for the given key.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func decode(
    _ type: Int128.Type,
    forKey key: KeyedDecodingContainer.Key
) throws -> Int128
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

