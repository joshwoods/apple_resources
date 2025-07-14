

- Swift
- KeyedEncodingContainer
-  nestedContainer(keyedBy:forKey:) 

Instance Method

# nestedContainer(keyedBy:forKey:)

Stores a keyed encoding container for the given key and returns it.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func nestedContainer(
    keyedBy keyType: NestedKey.Type,
    forKey key: KeyedEncodingContainer.Key
) -> KeyedEncodingContainer where NestedKey : CodingKey
```

## Parameters 

`keyType`  

The key type to use for the container.

`key`  

The key to encode the container for.

## Return Value

A new keyed encoding container.

