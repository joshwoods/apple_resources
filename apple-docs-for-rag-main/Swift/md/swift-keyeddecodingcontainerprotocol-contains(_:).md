

- Swift
- KeyedDecodingContainerProtocol
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the decoder contains a value associated with the given key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contains(_ key: Self.Key) -> Bool
```

**Required**

## Parameters 

`key`  

The key to search for.

## Return Value

Whether the `Decoder` has an entry for the given key.

## Discussion

The value associated with `key` may be a null value as appropriate for the data format.

