

- Core ML
- MLShapedArray
-  encode(to:) 

Instance Method

# encode(to:)

Encode a shaped array.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func encode(to encoder: any Encoder) throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `Encodable`.

## Parameters 

`encoder`  

The object to encode the shaped array.

## See Also

### Encoding and decoding

init(from: any Decoder) throws

Creates a shaped array from a decoder.

