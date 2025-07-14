

- Swift
- KeyedEncodingContainerProtocol
-  superEncoder(forKey:) 

Instance Method

# superEncoder(forKey:)

Stores a new nested container for the given key and returns a new encoder instance for encoding `super` into that container.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func superEncoder(forKey key: Self.Key) -> any Encoder
```

**Required**

## Parameters 

`key`  

The key to encode `super` for.

## Return Value

A new encoder to pass to `super.encode(to:)`.

