

- Swift
- KeyedDecodingContainer
-  decodeIfPresent(\_:forKey:) 

Instance Method

# decodeIfPresent(\_:forKey:)

Decodes a value of the given type for the given key, if present.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decodeIfPresent(
    _ type: UInt64.Type,
    forKey key: KeyedDecodingContainer.Key
) throws -> UInt64?
```

## Parameters 

`type`  

The type of value to decode.

`key`  

The key that the decoded value is associated with.

## Return Value

A decoded value of the requested type, or `nil` if the `Decoder` does not have an entry associated with the given key, or if the value is a null value.

## Discussion

This method returns `nil` if the container does not have a value associated with `key`, or if the value is null. The difference between these states can be distinguished with a `contains(_:)` call.

Throws

`DecodingError.typeMismatch` if the encountered encoded value is not convertible to the requested type.

