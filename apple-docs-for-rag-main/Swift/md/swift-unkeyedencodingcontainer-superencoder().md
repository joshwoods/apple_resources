

- Swift
- UnkeyedEncodingContainer
-  superEncoder() 

Instance Method

# superEncoder()

Encodes a nested container and returns an `Encoder` instance for encoding `super` into that container.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func superEncoder() -> any Encoder
```

**Required**

## Return Value

A new encoder to pass to `super.encode(to:)`.

