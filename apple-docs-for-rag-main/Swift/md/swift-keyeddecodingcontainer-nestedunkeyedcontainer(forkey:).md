

- Swift
- KeyedDecodingContainer
-  nestedUnkeyedContainer(forKey:) 

Instance Method

# nestedUnkeyedContainer(forKey:)

Returns the data stored for the given key as represented in an unkeyed container.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func nestedUnkeyedContainer(forKey key: KeyedDecodingContainer.Key) throws -> any UnkeyedDecodingContainer
```

## Parameters 

`key`  

The key that the nested container is associated with.

## Return Value

An unkeyed decoding container view into `self`.

## Discussion

Throws

`DecodingError.typeMismatch` if the encountered stored value is not an unkeyed container.

