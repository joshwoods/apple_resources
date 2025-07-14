

- Swift
- Decoder
-  container(keyedBy:) 

Instance Method

# container(keyedBy:)

Returns the data stored in this decoder as represented in a container keyed by the given key type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func container(keyedBy type: Key.Type) throws -> KeyedDecodingContainer where Key : CodingKey
```

**Required**

## Parameters 

`type`  

The key type to use for the container.

## Return Value

A keyed decoding container view into this decoder.

## Discussion

Throws

`DecodingError.typeMismatch` if the encountered stored value is not a keyed container.

