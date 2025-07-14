

- Accelerate
- vImage
- vImage Operations
-  Image rotation 

API Collection

# Image rotation

Rotate images by arbitrary angles or by multiples of 90 degrees.

## Topics

### Rotating 8-bit-per-channel buffers by any angle

func vImageRotate_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Float, Pixel_8, vImage_Flags) -> vImage_Error

Rotates an 8-bit planar image by any angle, which you specify in radians.

func vImageRotate_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Float, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Rotates an 8-bit-per-channel, 4-channel interleaved image by any angle, which you specify in radians.

### Rotating 16-bit-per-channel buffers by any angle

func vImageRotate_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Float, Pixel_16F, vImage_Flags) -> vImage_Error

Rotates a floating-point 16-bit planar image by any angle, which you specify in radians.

func vImageRotate_CbCr16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Float, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Rotates a floating-point 16-bit-per-channel, 2-channel interleaved image by any angle, which you specify in radians.

func vImageRotate_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Float, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Rotates an unsigned 16-bit-per-channel, 4-channel interleaved image by any angle, which you specify in radians.

func vImageRotate_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Float, UnsafePointer&lt;Int16>!, vImage_Flags) -> vImage_Error

Rotates a signed 16-bit-per-channel, 4-channel interleaved image by any angle, which you specify in radians.

func vImageRotate_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Float, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Rotates a floating-point 16-bit-per-channel, 4-channel interleaved image by any angle, which you specify in radians.

### Rotating 32-bit-per-channel buffers by any angle

func vImageRotate_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Float, Pixel_F, vImage_Flags) -> vImage_Error

Rotates a 32-bit planar image by any angle, which you specify in radians.

func vImageRotate_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, Float, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Rotates a 32-bit-per-channel, 4-channel interleaved image by any angle, which you specify in radians.

### Rotating 8-bit-per-channel buffers by multiples of 90°

func vImageRotate90_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, Pixel_8, vImage_Flags) -> vImage_Error

Rotates an 8-bit planar image by a multiple of 90°.

func vImageRotate90_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Rotates an 8-bit-per-channel, 4-channel interleaved image by a multiple of 90°.

### Rotating 16-bit-per-channel buffers by multiples of 90°

func vImageRotate90_Planar16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, Pixel_16U, vImage_Flags) -> vImage_Error

Rotates an unsigned 16-bit planar image by a multiple of 90°.

func vImageRotate90_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, Pixel_16F, vImage_Flags) -> vImage_Error

Rotates a floating-point 16-bit planar image by a multiple of 90°.

func vImageRotate90_CbCr16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Rotates a floating-point 16-bit-per-channel, 2-channel interleaved image by a multiple of 90°.

func vImageRotate90_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, UnsafePointer&lt;UInt16>, vImage_Flags) -> vImage_Error

Rotates an unsigned 16-bit-per-channel, 4-channel interleaved image by a multiple of 90°.

func vImageRotate90_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, UnsafePointer&lt;Int16>, vImage_Flags) -> vImage_Error

Rotates a signed 16-bit-per-channel, 4-channel interleaved image by a multiple of 90°.

func vImageRotate90_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Rotates a floating-point 16-bit-per-channel, 4-channel interleaved image by a multiple of 90°.

### Rotating 32-bit-per-channel buffers by multiples of 90°

func vImageRotate90_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, Pixel_F, vImage_Flags) -> vImage_Error

Rotates a 32-bit planar image by a multiple of 90°.

func vImageRotate90_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, UnsafePointer&lt;Float>, vImage_Flags) -> vImage_Error

Rotates a 32-bit-per-channel, 4-channel interleaved image by a multiple of 90°.

### Specifying the angle of a multiple of 90° rotation

Rotation constants

The number of degrees to rotate an image.

## See Also

### Applying geometric transforms to image buffers

Resampling in vImage

Learn how vImage resamples image data during geometric operations.

Applying affine transformations to images

Translate, rotate, and scale images.

Applying projective transformations to images

Warp images in three dimensions.

Image reflection

Reflect images horizontally and vertically.

Image shearing

Shear images horizontally and vertically.

Image scaling

Scale interlaced and planar images.

Getting the Buffer Size

Calculate the size of the temporary buffer needed by a high-level geometry functions.

