

- Swift
- UnkeyedDecodingContainer
-  nestedUnkeyedContainer() 

Instance Method

# nestedUnkeyedContainer()

Decodes an unkeyed nested container.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func nestedUnkeyedContainer() throws -> any UnkeyedDecodingContainer
```

**Required**

## Return Value

An unkeyed decoding container view into `self`.

## Discussion

Throws

`DecodingError.typeMismatch` if the encountered stored value is not an unkeyed container.

