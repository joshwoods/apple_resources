

- Swift
- Encoder
-  container(keyedBy:) 

Instance Method

# container(keyedBy:)

Returns an encoding container appropriate for holding multiple values keyed by the given key type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func container(keyedBy type: Key.Type) -> KeyedEncodingContainer where Key : CodingKey
```

**Required**

## Parameters 

`type`  

The key type to use for the container.

## Return Value

A new keyed encoding container.

## Discussion

You must use only one kind of top-level encoding container. This method must not be called after a call to `unkeyedContainer()` or after encoding a value through a call to `singleValueContainer()`

