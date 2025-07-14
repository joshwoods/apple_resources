

- Core ML
- MLShapedArraySlice
-  init(from:) 

Initializer

# init(from:)

Creates an array slice from the passed decoder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(from decoder: any Decoder) throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `Decodable`.

## Parameters 

`decoder`  

The object that decodes the array slice for initialization.

## See Also

### Encoding and Decoding an Array Slice

func encode(to: any Encoder) throws

Encodes the array slice.

