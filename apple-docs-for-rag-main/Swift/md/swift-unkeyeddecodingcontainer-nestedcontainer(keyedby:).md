

- Swift
- UnkeyedDecodingContainer
-  nestedContainer(keyedBy:) 

Instance Method

# nestedContainer(keyedBy:)

Decodes a nested container keyed by the given type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func nestedContainer(keyedBy type: NestedKey.Type) throws -> KeyedDecodingContainer where NestedKey : CodingKey
```

**Required**

## Parameters 

`type`  

The key type to use for the container.

## Return Value

A keyed decoding container view into `self`.

## Discussion

Throws

`DecodingError.typeMismatch` if the encountered stored value is not a keyed container.

