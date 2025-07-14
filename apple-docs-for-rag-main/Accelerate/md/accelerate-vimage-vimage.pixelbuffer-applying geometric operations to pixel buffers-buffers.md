

- Accelerate
- vImage
- vImage.PixelBuffer
-  Applying geometric operations to pixel buffers 

API Collection

# Applying geometric operations to pixel buffers

Reflect, shear, rotate, scale, and apply affine transforms to image data.

## Topics

### Reflecting images

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects an 8-bit planar pixel buffer over a horizontal or vertical axis.

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects a floating-point 16-bit planar pixel buffer over a horizontal or vertical axis.

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects a 32-bit planar pixel buffer over a horizontal or vertical axis.

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects a floating-point 16-bit-per-channel, two-channel interleaved pixel buffer over a horizontal or vertical axis.

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects an 8-bit-per-channel, four-channel interleaved pixel buffer over a horizontal or vertical axis.

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects an unsigned 16-bit-per-channel, four-channel interleaved pixel buffer over a horizontal or vertical axis.

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects a floating-point 16-bit-per-channel, four-channel interleaved pixel buffer over a horizontal or vertical axis.

func reflect(over: vImage.ReflectionAxis, destination: vImage.PixelBuffer&lt;Format>)

Reflects a 32-bit-per-channel, four-channel interleaved pixel buffer over a horizontal or vertical axis.

enum ReflectionAxis

The axis to reflect an image.

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

func rotate(vImage.Rotation, backgroundColor: Pixel_ARGB_16F?, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Rotates a floating-point 16-bit-per-channel, four-channel interleaved pixel buffer.

func rotate(vImage.Rotation, backgroundColor: Pixel_FFFF?, destination: vImage.PixelBuffer&lt;Format>)

Rotates a 32-bit-per-channel, four-channel interleaved pixel buffer.

enum Rotation

The angle to rotate an image.

### Scaling images

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales an 8-bit planar pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales an unsigned 16-bit planar pixel buffer to fit the destination buffer.

func scale(useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Scales a floating-point 16-bit planar pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales a 32-bit planar pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales an 8-bit-per-channel, two-channel interleaved pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales an unsigned 16-bit-per-channel, two-channel interleaved pixel buffer to fit the destination buffer.

func scale(useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Scales a floating-point 16-bit-per-channel, two-channel interleaved pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales an 8-bit-per-channel, four-channel interleaved pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales an unsigned 16-bit-per-channel, four-channel interleaved pixel buffer to fit the destination buffer.

func scale(useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Scales a floating-point 16-bit-per-channel, four-channel interleaved pixel buffer to fit the destination buffer.

func scale(destination: vImage.PixelBuffer&lt;Format>)

Scales a 32-bit-per-channel, four-channel interleaved pixel buffer to fit the destination buffer.

### Shearing images

func shear&lt;T>(direction: vImage.ShearDirection, translate: T, slope: T, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_8?, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on an 8-bit planar pixel buffer.

func shear(direction: vImage.ShearDirection, translate: Float, slope: Float, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_16U?, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on an unsigned 16-bit planar pixel buffer.

func shear&lt;T>(direction: vImage.ShearDirection, translate: T, slope: T, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_16F?, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on a floating-point 16-bit planar pixel buffer.

func shear&lt;T>(direction: vImage.ShearDirection, translate: T, slope: T, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_F?, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on a 32-bit planar pixel buffer.

func shear&lt;T>(direction: vImage.ShearDirection, translate: T, slope: T, resamplingFilter: ResamplingFilter, backgroundColor: Pixel_16U16U?, destination: vImage.PixelBuffer&lt;Format>)

Performs a horizontal or vertical shear operation on an unsigned 16-bit-per-channel, two-channel interleaved pixel buffer.

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

### Applying affine transformations to images

func transform(CGAffineTransform, backgroundColor: Pixel_8?, destination: vImage.PixelBuffer&lt;Format>)

Applies a Core Graphics affine transformation to an 8-bit planar pixel buffer.

func transform(CGAffineTransform, backgroundColor: Pixel_16F?, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Applies a Core Graphics affine transformation to a floating-point 16-bit planar pixel buffer.

func transform(CGAffineTransform, backgroundColor: Pixel_F?, destination: vImage.PixelBuffer&lt;Format>)

Applies a Core Graphics affine transformation to a floating-point 32-bit planar pixel buffer.

func transform(CGAffineTransform, backgroundColor: Pixel_16F16F?, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Applies a Core Graphics affine transformation to a floating-point 16-bit-per-channel, two-channel interleaved pixel buffer.

func transform(CGAffineTransform, backgroundColor: Pixel_8888?, destination: vImage.PixelBuffer&lt;Format>)

Applies a Core Graphics affine transformation to an 8-bit-per-channel, four-channel interleaved pixel buffer.

func transform(CGAffineTransform, backgroundColor: Pixel_ARGB_16U?, destination: vImage.PixelBuffer&lt;Format>)

Applies a Core Graphics affine transformation to an unsigned 16-bit-per-channel, four-channel interleaved pixel buffer.

func transform(CGAffineTransform, backgroundColor: Pixel_ARGB_16F?, useFloat16Accumulator: Bool, destination: vImage.PixelBuffer&lt;Format>)

Applies a Core Graphics affine transformation to a floating-point 16-bit-per-channel, four-channel interleaved pixel buffer.

func transform(CGAffineTransform, backgroundColor: Pixel_FFFF?, destination: vImage.PixelBuffer&lt;Format>)

Applies a Core Graphics affine transformation to a floating-point 32-bit-per-channel, four-channel interleaved pixel buffer.

### Applying projective transformations to images

func transform(vImage_PerpsectiveTransform, interpolation: vImage_PerpsectiveTransform.Interpolation, backgroundColor: Pixel_8, destination: vImage.PixelBuffer&lt;Format>)

Applies a perspective warp to an 8-bit planar image.

func transform(vImage_PerpsectiveTransform, interpolation: vImage_PerpsectiveTransform.Interpolation, backgroundColor: Pixel_8888, destination: vImage.PixelBuffer&lt;Format>)

Applies a perspective warp to an interleaved 4-channel, 8-bit planar image.

func transform(vImage_PerpsectiveTransform, interpolation: vImage_PerpsectiveTransform.Interpolation, backgroundColor: Pixel_16U, destination: vImage.PixelBuffer&lt;Format>)

Applies a perspective warp to an unsigned-integer 16-bit planar image.

func transform(vImage_PerpsectiveTransform, interpolation: vImage_PerpsectiveTransform.Interpolation, backgroundColor: Pixel_ARGB_16U, destination: vImage.PixelBuffer&lt;Format>)

Applies a perspective warp to an interleaved 4-channel, unsigned 16-bit planar image.

func transform(vImage_PerpsectiveTransform, interpolation: vImage_PerpsectiveTransform.Interpolation, backgroundColor: Pixel_16F, destination: vImage.PixelBuffer&lt;Format>)

Applies a perspective warp to a floating-point 16-bit planar image.

func transform(vImage_PerpsectiveTransform, interpolation: vImage_PerpsectiveTransform.Interpolation, backgroundColor: Pixel_ARGB_16F, destination: vImage.PixelBuffer&lt;Format>)

Applies a perspective warp to an interleaved 4-channel, floating-point 16-bit planar image.

## See Also

### Pixel buffer operations

Applying color transforms to pixel buffers

Adjust the colors of an image by applying gamma, polynomials, or multidimensional lookup.

Blending and compositing pixel buffers

Composite two pixel buffers to create a single image.

Convolving and applying morphology

Apply convolution, dilation, or erosion to a pixel buffer.

Thresholding and clipping pixel buffer values

Limit the values in a pixel buffer to a threshold or a range.

Calculating and transforming histograms

Enhance and adjust the contrast of an image with histogram equalization, contrast stretching, and specification.

Converting pixel buffers

Convert pixel buffer data between different bit-depths.

Interleaving and deinterleaving pixel buffers

Convert pixel buffer data between interleaved and planar formats.

Cropping and working with regions of interest

Crop images and apply operations to regions of interest.

Applying channel operations

Extract, flatten, permute, and overwrite the individual color channels of a pixel buffer.

Applying arithmetic operations

Multiply the pixel values of a buffer by scalar values or matrices.

