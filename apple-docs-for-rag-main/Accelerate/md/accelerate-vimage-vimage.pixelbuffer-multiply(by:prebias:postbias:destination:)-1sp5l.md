

- Accelerate
- vImage
- vImage.PixelBuffer
-  multiply(by:preBias:postBias:destination:) 

Instance Method

# multiply(by:preBias:postBias:destination:)

Multiplies each four channel pixel in a 32-bit-per channel, 4-channel pixel buffer by a four element matrix to produce a single channel result.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func multiply(
    by matrix: (Float, Float, Float, Float),
    preBias: (Float, Float, Float, Float),
    postBias: Float,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.InterleavedFx4`.

## Parameters 

`matrix`  

The 4 x 4 multiplication matrix values in row-major order.

`preBias`  

Values that the function adds to the source before multiplication.

`postBias`  

A value that the function adds to the result after multiplication.

`destination`  

The destination pixel buffer.

## Discussion

This function applies the following operation to each pixel:

```
p = (source.0 + preBias.0) * matrix.0 +
    (source.1 + preBias.1) * matrix.1 +
    (source.2 + preBias.2) * matrix.2 +
    (source.3 + preBias.3) * matrix.3
destination = (p + postBias)
```

## See Also

### Pixel Multiplication

func multiply(by: (Int, Int, Int, Int), divisor: Int, preBias: (Int, Int, Int, Int), postBias: Int, destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Multiplies each four channel pixel in an 8-bit-per channel, 4-channel pixel buffer by a four element matrix to produce a single channel result.

