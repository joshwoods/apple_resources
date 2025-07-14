

- Accelerate
- vImage
- vImage Operations
-  Applying projective transformations to images 

API Collection

# Applying projective transformations to images

Warp images in three dimensions.

## Topics

### Computing a projective transformation from source and destination quadrilaterals

Transforming an image in three dimensions

Create and use a projective transformation to apply a perspective warp to an image.

func vImageGetPerspectiveWarp(UnsafePointer&lt;(Float, Float)>, UnsafePointer&lt;(Float, Float)>, UnsafeMutablePointer&lt;vImage_PerpsectiveTransform>, vImage_Flags) -> vImage_Error

Returns a projective-transformation structure that defines the mapping between a source quadrilateral and a destination quadrilateral.

struct vImage_PerpsectiveTransform

A projective-transformation matrix.

### Warping planar buffers

func vImagePerspectiveWarp_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_PerpsectiveTransform>, vImage_WarpInterpolation, Pixel_8, vImage_Flags) -> vImage_Error

Applies a perspective warp to an 8-bit planar image.

func vImagePerspectiveWarp_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_PerpsectiveTransform>, vImage_WarpInterpolation, Pixel_16F, vImage_Flags) -> vImage_Error

Applies a perspective warp to a floating-point 16-bit planar image.

func vImagePerspectiveWarp_Planar16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_PerpsectiveTransform>, vImage_WarpInterpolation, Pixel_16U, vImage_Flags) -> vImage_Error

Applies a perspective warp to a unsigned 16-bit planar image.

### Warping interleaved buffers

func vImagePerspectiveWarp_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_PerpsectiveTransform>, vImage_WarpInterpolation, UnsafeMutablePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Applies a perspective warp to an 8-bit-per-channel, four-channel interleaved image.

func vImagePerspectiveWarp_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_PerpsectiveTransform>, vImage_WarpInterpolation, UnsafeMutablePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a perspective warp to a floating-point 16-bit , four-channel interleaved image.

func vImagePerspectiveWarp_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_PerpsectiveTransform>, vImage_WarpInterpolation, UnsafeMutablePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a perspective warp to an unsigned 16-bit , four-channel interleaved image.

## See Also

### Applying geometric transforms to image buffers

Resampling in vImage

Learn how vImage resamples image data during geometric operations.

Applying affine transformations to images

Translate, rotate, and scale images.

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

