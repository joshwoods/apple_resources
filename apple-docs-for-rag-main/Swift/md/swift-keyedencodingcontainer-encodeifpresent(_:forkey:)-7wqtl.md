

- Swift
- KeyedEncodingContainer
-  encodeIfPresent(\_:forKey:) 

Instance Method

# encodeIfPresent(\_:forKey:)

Encodes the given value for the given key if it is not `nil`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func encodeIfPresent(
    _ value: Int128?,
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

