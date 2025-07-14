

- Swift
- KeyedDecodingContainer
-  superDecoder(forKey:) 

Instance Method

# superDecoder(forKey:)

Returns a `Decoder` instance for decoding `super` from the container associated with the given key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func superDecoder(forKey key: KeyedDecodingContainer.Key) throws -> any Decoder
```

## Parameters 

`key`  

The key to decode `super` for.

## Return Value

A new `Decoder` to pass to `super.init(from:)`.

## Discussion

Throws

`DecodingError.keyNotFound` if `self` does not have an entry for the given key.

Throws

`DecodingError.valueNotFound` if `self` has a null entry for the given key.

