

- Swift
- UnkeyedEncodingContainer
-  nestedContainer(keyedBy:) 

Instance Method

# nestedContainer(keyedBy:)

Encodes a nested container keyed by the given type and returns it.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func nestedContainer(keyedBy keyType: NestedKey.Type) -> KeyedEncodingContainer where NestedKey : CodingKey
```

**Required**

## Parameters 

`keyType`  

The key type to use for the container.

## Return Value

A new keyed encoding container.

