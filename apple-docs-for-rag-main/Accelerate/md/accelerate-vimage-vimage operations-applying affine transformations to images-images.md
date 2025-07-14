

- Accelerate
- vImage
- vImage Operations
-  Applying affine transformations to images 

API Collection

# Applying affine transformations to images

Translate, rotate, and scale images.

## Topics

### Single-Precision Affine Transformation

func vImageAffineWarp_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, Pixel_8, vImage_Flags) -> vImage_Error

Applies a single-precision affine transformation to an 8-bit planar image.

func vImageAffineWarp_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, Pixel_F, vImage_Flags) -> vImage_Error

Applies a single-precision affine transformation to a 32-bit planar image.

func vImageAffineWarp_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a single-precision affine transformation to an unsigned 16-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarp_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, UnsafePointer&lt;Int16>!, vImage_Flags) -> vImage_Error

Applies a single-precision affine transformation to a signed 16-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarp_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Applies a single-precision affine transformation to an 8-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarp_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Applies a single-precision affine transformation to a 32-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarp_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

func vImageAffineWarp_CbCr16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

func vImageAffineWarp_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, Pixel_16F, vImage_Flags) -> vImage_Error

### Double-Precision Affine Transformation

func vImageAffineWarpD_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, Pixel_8, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to an 8-bit planar image.

func vImageAffineWarpD_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, Pixel_F, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to a 32-bit planar image.

func vImageAffineWarpD_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, Pixel_16F, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to a floating-point 16-bit planar image.

func vImageAffineWarpD_CbCr16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to a floating-point 16-bit-per-channel, 2-channel interleaved image.

func vImageAffineWarpD_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to an 8-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarpD_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to an unsigned 16-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarpD_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, UnsafePointer&lt;Int16>!, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to a signed 16-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarpD_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to a floating-point 16-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarpD_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform_Double>, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Applies a double-precision affine transformation to a 32-bit-per-channel, 4-channel interleaved image.

### Core Graphics Affine Transformation

func vImageAffineWarpCG_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_CGAffineTransform>, Pixel_8, vImage_Flags) -> vImage_Error

Applies a Core Graphics affine transformation to a Planar8 source image.

func vImageAffineWarpCG_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_CGAffineTransform>, Pixel_F, vImage_Flags) -> vImage_Error

Applies a Core Graphics affine transformation to a PlanarF source image.

func vImageAffineWarpCG_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_CGAffineTransform>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a Core Graphics affine transformation to an ARGB16U source image.

func vImageAffineWarpCG_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_CGAffineTransform>, UnsafePointer&lt;Int16>!, vImage_Flags) -> vImage_Error

Applies a Core Graphics affine transformation to an ARGB16S source image.

func vImageAffineWarpCG_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_CGAffineTransform>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Applies a Core Graphics affine transformation to an ARGB8888 source image.

func vImageAffineWarpCG_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_CGAffineTransform>, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Applies a Core Graphics affine transformation to an ARGBFFFF source image.

## See Also

### Applying geometric transforms to image buffers

Resampling in vImage

Learn how vImage resamples image data during geometric operations.

Applying projective transformations to images

Warp images in three dimensions.

Image reflection

Reflect images horizontally and vertically.

Image shearing

Shear images horizontally and vertically.

Image rotation

Rotate images by arbitrary angles or by multiples of 90 degrees.

Image scaling

Scale interlaced and planar images.

Getting the Buffer Size

Calculate the size of the temporary buffer needed by a high-level geometry functions.

