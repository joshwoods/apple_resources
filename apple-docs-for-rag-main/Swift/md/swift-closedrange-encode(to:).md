

- Swift
- ClosedRange
-  encode(to:) 

Instance Method

# encode(to:)

Encodes this value into the given encoder.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func encode(to encoder: any Encoder) throws
```

Available when `Bound` conforms to `Comparable` and `Encodable`.

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

If the value fails to encode anything, `encoder` will encode an empty keyed container in its place.

This function throws an error if any values are invalid for the given encoder’s format.

## See Also

### Encoding and Decoding a Range

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

