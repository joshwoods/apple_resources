

- Swift
- KeyedDecodingContainerProtocol
-  decodeNil(forKey:) 

Instance Method

# decodeNil(forKey:)

Decodes a null value for the given key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decodeNil(forKey key: Self.Key) throws -> Bool
```

**Required**

## Parameters 

`key`  

The key that the decoded value is associated with.

## Return Value

Whether the encountered value was null.

## Discussion

Throws

`DecodingError.keyNotFound` if `self` does not have an entry for the given key.

