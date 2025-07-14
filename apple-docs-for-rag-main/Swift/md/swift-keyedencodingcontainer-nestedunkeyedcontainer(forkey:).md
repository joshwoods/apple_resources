

- Swift
- KeyedEncodingContainer
-  nestedUnkeyedContainer(forKey:) 

Instance Method

# nestedUnkeyedContainer(forKey:)

Stores an unkeyed encoding container for the given key and returns it.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func nestedUnkeyedContainer(forKey key: KeyedEncodingContainer.Key) -> any UnkeyedEncodingContainer
```

## Parameters 

`key`  

The key to encode the container for.

## Return Value

A new unkeyed encoding container.

