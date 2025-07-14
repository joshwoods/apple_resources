

- Accelerate
- vImage
- vImage.PixelBuffer
-  multiply(by:preBias:postBias:destination:) 

Instance Method

# multiply(by:preBias:postBias:destination:)

Multiplies each pixel in a 32-bit planar pixel buffer by the specified factor.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func multiply(
    by factor: Float,
    preBias: Float,
    postBias: Float,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.PlanarF`.

## Parameters 

`factor`  

The multiplication factor.

`preBias`  

A value that the function adds to the source before multiplication.

`postBias`  

A value that the function adds to the result after multiplication.

`destination`  

The destination pixel buffer.

## Discussion

This function applies the following operation to each pixel:

```
destination = ((source + preBias) * factor) + postBias
```

For example, the following code multiplies each pixel value in a 32-bit planar buffer by `2`:

```
   let buffer = vImage.PixelBuffer(
       pixelValues: [0.1, 0.2, 0.3, 0.4, 0.5],
       size: vImage.Size(width: 5,
                         height: 1))

   buffer.multiply(by: 2,
                   preBias: 0, postBias: 0,
                   destination: buffer)

   // Prints "[0.2, 0.4, 0.6, 0.8, 1.0]"
   print(buffer.array)
```

## See Also

### Scalar Multiplication

func multiply(by: Int, divisor: Int, preBias: Int, postBias: Int, destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Multiplies each pixel in an 8-bit planar pixel buffer by the specified factor.

