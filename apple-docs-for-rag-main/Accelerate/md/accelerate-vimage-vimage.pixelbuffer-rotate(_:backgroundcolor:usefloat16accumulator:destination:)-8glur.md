

- Accelerate
- vImage
- vImage.PixelBuffer
-  rotate(\_:backgroundColor:useFloat16Accumulator:destination:) 

Instance Method

# rotate(\_:backgroundColor:useFloat16Accumulator:destination:)

Rotates a floating-point 16-bit-per-channel, four-channel interleaved pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func rotate(
    _ rotation: vImage.Rotation,
    backgroundColor: Pixel_ARGB_16F? = (0, 0, 0, 0),
    useFloat16Accumulator: Bool = false,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Interleaved16Fx4`.

## Parameters 

`rotation`  

An enumeration that specifies the rotation angle.

`backgroundColor`  

An optional background color. If you pass `nil`, the operation uses the kvImageEdgeExtend flag to extend the edges of the image infinitely.

`useFloat16Accumulator`  

A Boolean value that specifies that the function uses faster, but lower-precision, internal arithmetic. For more information, see kvImageUseFP16Accumulator.

`destination`  

The destination pixel buffer.

## Discussion

Use this function to either rotate an image by a multiple of 90° or by an angle, which you specify in degrees or radians.

When you specify a rotation that’s a multiple of 90° (such as vImage.Rotation.clockwise270Degrees), this function maps the center point of the source image to the center point of the destination image. It doesn’t scale or resample; instead, the function copies individual pixels unchanged to new locations.

The 90° and 270° rotations don’t rotate around the true center of the image if either of the following is true:

- The parities of the source height and the destination width don’t match. For example, the source height is odd and the destination width is even.

- The parities of the source width and the destination height don’t match. For example, the source width is odd and the destination height is even.

The 0° and 180° rotations don’t rotate around the true center of the image if either of the following is true:

- The parities of the source height and the destination height don’t match. For example, the source height is odd and the destination height is even.

- The parities of the source width and the destination width don’t match. For example, the source width is odd and the destination width is even.

To overcome this limitation, specify vImage.Rotation.angleInRadians(_:) or vImage.Rotation.angleInDegrees(_:) to invoke the high-level rotate function.

## See Also

### Related Documentation

Applying geometric transforms to images

Reflect, shear, rotate, and scale image buffers using vImage.

### Rotating images

func rotate(vImage.Rotation, backgroundColor: Pixel_8?, destination: vImage.PixelBuffer&lt;Format>)

Rotates an 8-bit planar pixel buffer.

func rotate(vImage.Rotation, backgroundColor: Pixel_16F?, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Rotates a floating-point 16-bit planar pixel buffer.

func rotate(vImage.Rotation, backgroundColor: Pixel_F?, destination: vImage.PixelBuffer&lt;Format>)

Rotates a 32-bit planar pixel buffer.

func rotate(vImage.Rotation, backgroundColor: Pixel_16F16F?, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Rotates a floating-point 16-bit-per-channel, two-channel interleaved pixel buffer.

func rotate(vImage.Rotation, backgroundColor: Pixel_8888?, destination: vImage.PixelBuffer&lt;Format>)

Rotates an 8-bit-per-channel, four-channel interleaved pixel buffer.

func rotate(vImage.Rotation, backgroundColor: Pixel_ARGB_16U?, destination: vImage.PixelBuffer&lt;Format>)

Rotates an unsigned 16-bit-per-channel, four-channel interleaved pixel buffer.

func rotate(vImage.Rotation, backgroundColor: Pixel_FFFF?, destination: vImage.PixelBuffer&lt;Format>)

Rotates a 32-bit-per-channel, four-channel interleaved pixel buffer.

enum Rotation

The angle to rotate an image.

