

- Swift
- KeyedEncodingContainer
-  encode(\_:forKey:) 

Instance Method

# encode(\_:forKey:)

Encodes the given value for the given key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func encode(
    _ value: UInt8,
    forKey key: KeyedEncodingContainer.Key
) throws
```

## Parameters 

`value`  

The value to encode.

`key`  

The key to associate the value with.

## Discussion

Throws

`EncodingError.invalidValue` if the given value is invalid in the current context for this format.

