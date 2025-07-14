

- Accelerate
- vImage
- vImage.PixelBuffer
-  shear(direction:translate:slope:resamplingFilter:backgroundColor:destination:) 

Instance Method

# shear(direction:translate:slope:resamplingFilter:backgroundColor:destination:)

Performs a horizontal or vertical shear operation on an unsigned 16-bit-per-channel, two-channel interleaved pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func shear(
    direction: vImage.ShearDirection,
    translate: T,
    slope: T,
    resamplingFilter: ResamplingFilter,
    backgroundColor: Pixel_16U16U? = (0, 0),
    destination: vImage.PixelBuffer
) where T : BinaryFloatingPoint
```

Available when `Format` is `vImage.Interleaved16Ux2`.

## Parameters 

`direction`  

An enumeration that specifies the shear direction.

`translate`  

A value that specifies the translation.

`slope`  

The slope of the front edge of the sheared image.

`resamplingFilter`  

The resampling filter that the function uses. For more information, see Reducing artifacts with custom resampling filters.

`backgroundColor`  

An optional background color. If you pass `nil`, the operation uses the kvImageEdgeExtend flag to extend the edges of the image infinitely.

`destination`  

The destination pixel buffer.

## See Also

### Related Documentation

Applying geometric transforms to images

Reflect, shear, rotate, and scale image buffers using vImage.

### Shearing images

func shear&lt;T>(direction: vImage.ShearDirection, translate: T, slope: T, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_8?, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on an 8-bit planar pixel buffer.

func shear(direction: vImage.ShearDirection, translate: Float, slope: Float, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_16U?, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on an unsigned 16-bit planar pixel buffer.

func shear&lt;T>(direction: vImage.ShearDirection, translate: T, slope: T, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_16F?, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on a floating-point 16-bit planar pixel buffer.

func shear&lt;T>(direction: vImage.ShearDirection, translate: T, slope: T, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_F?, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on a 32-bit planar pixel buffer.

func shear(direction: vImage.ShearDirection, translate: Float, slope: Float, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_88?, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on an 8-bit-per-channel, two-channel interleaved pixel buffer.

func shear&lt;T>(direction: vImage.ShearDirection, translate: T, slope: T, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_16F16F?, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on a floating-point 16-bit-per-channel, two-channel interleaved pixel buffer.

func shear&lt;T>(direction: vImage.ShearDirection, translate: T, slope: T, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_8888?, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on an 8-bit-per-channel, four-channel interleaved pixel buffer.

func shear&lt;T>(direction: vImage.ShearDirection, translate: T, slope: T, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_ARGB_16U?, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on an unsigned 16-bit-per-channel, four-channel interleaved pixel buffer.

func shear&lt;T>(direction: vImage.ShearDirection, translate: T, slope: T, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_ARGB_16F?, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on a floating-point 16-bit-per-channel, four-channel interleaved pixel buffer.

func shear&lt;T>(direction: vImage.ShearDirection, translate: T, slope: T, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_FFFF?, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on a 32-bit-per-channel, four-channel interleaved pixel buffer.

enum ShearDirection

The shear direction.

