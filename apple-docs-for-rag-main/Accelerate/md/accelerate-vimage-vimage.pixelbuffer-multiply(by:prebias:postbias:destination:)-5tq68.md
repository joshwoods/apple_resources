

- Accelerate
- vImage
- vImage.PixelBuffer
-  multiply(by:preBias:postBias:destination:) 

Instance Method

# multiply(by:preBias:postBias:destination:)

Multiplies each four channel pixel in a 32-bit-per channel, 4-channel pixel buffer by a 4 x 4 simd matrix to produce a four channel result.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func multiply(
    by matrix: simd_float4x4,
    preBias: (Float, Float, Float, Float),
    postBias: (Float, Float, Float, Float),
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

### Matrix Multiplication

func multiply&lt;Matrix>(by: Matrix, divisor: Int, preBias: (Int, Int, Int, Int), postBias: (Int, Int, Int, Int), destination: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Multiplies each four channel pixel in an 8-bit-per channel, 4-channel pixel buffer by a 4 x 4 matrix to produce a four channel result.

func multiply&lt;Matrix>(by: Matrix, preBias: (Float, Float, Float, Float), postBias: (Float, Float, Float, Float), destination: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Multiplies each four channel pixel in a 32-bit-per channel, 4-channel pixel buffer by a 4 x 4 matrix to produce a four channel result.

func multiply&lt;Matrix, DestFormat>(by: Matrix, divisor: Int, preBias: [Int], postBias: [Int], destination: vImage.PixelBuffer&lt;DestFormat>)

Multiplies each four channel pixel in an 8-bit multiple-plane pixel buffer by a 4 x 4 matrix to produce a four channel result.

func multiply&lt;Matrix, DestFormat>(by: Matrix, preBias: [Float], postBias: [Float], destination: vImage.PixelBuffer&lt;DestFormat>)

Multiplies each four channel pixel in a 32-bit multiple-plane pixel buffer by a 4 x 4 matrix to produce a four channel result.

