

- Swift
- KeyedDecodingContainerProtocol
-  nestedContainer(keyedBy:forKey:) 

Instance Method

# nestedContainer(keyedBy:forKey:)

Returns the data stored for the given key as represented in a container keyed by the given key type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func nestedContainer(
    keyedBy type: NestedKey.Type,
    forKey key: Self.Key
) throws -> KeyedDecodingContainer where NestedKey : CodingKey
```

**Required**

## Parameters 

`type`  

The key type to use for the container.

`key`  

The key that the nested container is associated with.

## Return Value

A keyed decoding container view into `self`.

## Discussion

Throws

`DecodingError.typeMismatch` if the encountered stored value is not a keyed container.

