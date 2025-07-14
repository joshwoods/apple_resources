

- Core ML
- MLShapedArray
-  init(from:) 

Initializer

# init(from:)

Creates a shaped array from a decoder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(from decoder: any Decoder) throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `Decodable`.

## Parameters 

`decoder`  

The decoder to read data from.

## Discussion

This initializer throws an error if reading from the decoder fails, or if the data read is corrupted or otherwise invalid.

## See Also

### Encoding and decoding

func encode(to: any Encoder) throws

Encode a shaped array.

