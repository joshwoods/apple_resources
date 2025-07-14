

- Swift
- UnkeyedDecodingContainer
-  superDecoder() 

Instance Method

# superDecoder()

Decodes a nested container and returns a `Decoder` instance for decoding `super` from that container.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func superDecoder() throws -> any Decoder
```

**Required**

## Return Value

A new `Decoder` to pass to `super.init(from:)`.

## Discussion

Throws

`DecodingError.valueNotFound` if the encountered encoded value is null, or of there are no more values to decode.

