

- Swift
- Decoder
-  unkeyedContainer() 

Instance Method

# unkeyedContainer()

Returns the data stored in this decoder as represented in a container appropriate for holding values with no keys.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func unkeyedContainer() throws -> any UnkeyedDecodingContainer
```

**Required**

## Return Value

An unkeyed container view into this decoder.

## Discussion

Throws

`DecodingError.typeMismatch` if the encountered stored value is not an unkeyed container.

