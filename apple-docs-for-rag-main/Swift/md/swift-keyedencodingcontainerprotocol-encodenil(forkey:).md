

- Swift
- KeyedEncodingContainerProtocol
-  encodeNil(forKey:) 

Instance Method

# encodeNil(forKey:)

Encodes a null value for the given key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func encodeNil(forKey key: Self.Key) throws
```

**Required**

## Parameters 

`key`  

The key to associate the value with.

## Discussion

Throws

`EncodingError.invalidValue` if a null value is invalid in the current context for this format.

