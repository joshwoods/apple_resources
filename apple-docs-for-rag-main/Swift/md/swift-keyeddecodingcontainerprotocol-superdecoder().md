

- Swift
- KeyedDecodingContainerProtocol
-  superDecoder() 

Instance Method

# superDecoder()

Returns a `Decoder` instance for decoding `super` from the container associated with the default `super` key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func superDecoder() throws -> any Decoder
```

**Required**

## Return Value

A new `Decoder` to pass to `super.init(from:)`.

## Discussion

Equivalent to calling `superDecoder(forKey:)` with `Key(stringValue: "super", intValue: 0)`.

Throws

`DecodingError.keyNotFound` if `self` does not have an entry for the default `super` key.

Throws

`DecodingError.valueNotFound` if `self` has a null entry for the default `super` key.

