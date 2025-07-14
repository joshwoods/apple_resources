

- Accelerate
- vImage
- vImage.PixelBuffer
-  applyGamma(linearParameters:exponentialParameters:boundary:destination:) 

Instance Method

# applyGamma(linearParameters:exponentialParameters:boundary:destination:)

Applies a piecewise gamma calculation to a 32-bit pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func applyGamma(
    linearParameters: (scale: Float, bias: Float),
    exponentialParameters: (scale: Float, preBias: Float, gamma: Float, postBias: Float),
    boundary: Float,
    destination: vImage.PixelBuffer
)
```

Available when `Format` conforms to `StaticPixelFormat` and `Format.ComponentType` is `Float`.

## Parameters 

`linearParameters`  

The scale and bias applied to pixels with a value below `boundary`.

`exponentialParameters`  

The boundary value that defines whether the function transforms pixels with the linear or the exponential calculation.

`boundary`  

The parameters that the function uses for the exponential calculation.

`destination`  

The destination pixel buffer.

## Discussion

This function computes the output value of each pixel using the following pseudocode:

```
For each source pixel value x:
 if x 

For example, the following code applies piecewise gamma to a one-pixel, two-channel pixel buffer.

The first channel’s value is below the boundary and the second channel’s value is above the boundary.

The operation mutliplies the first channel’s value by two and squares the second channel’s value.

```
let buffer = vImage.PixelBuffer(
    pixelValues: [0.25, 0.75],
    size: vImage.Size(width: 1,
                      height: 1))

buffer.applyGamma(linearParameters: (scale: 2,
                                     bias: 0),
                  exponentialParameters: (scale: 1,
                                          preBias: 0,
                                          gamma: 2,
                                          postBias: 0),
                  boundary: 0.5,
                  destination: buffer)

// Prints "[0.5, 0.5625]" = [ 0.25 * 2, 0.75² ].
print(buffer.array)
```

## See Also

### Applying piecewise gamma

func applyGamma(linearParameters: (scale: Float, bias: Float), exponentialParameters: (scale: Float, preBias: Float, gamma: Float, postBias: Float), boundary: Pixel_8, destination: vImage.PixelBuffer&lt;Format>)

Applies a piecewise gamma calculation to an 8-bit pixel buffer.

