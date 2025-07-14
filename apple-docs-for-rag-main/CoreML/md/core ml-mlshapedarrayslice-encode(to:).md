

- Core ML
- MLShapedArraySlice
-  encode(to:) 

Instance Method

# encode(to:)

Encodes the array slice.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func encode(to encoder: any Encoder) throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `Encodable`.

## Parameters 

`encoder`  

The object that encodes the array slice.

## See Also

### Encoding and Decoding an Array Slice

init(from: any Decoder) throws

Creates an array slice from the passed decoder.

