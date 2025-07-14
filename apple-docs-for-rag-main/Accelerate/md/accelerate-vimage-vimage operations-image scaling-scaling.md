

- Accelerate
- vImage
- vImage Operations
-  Image scaling 

API Collection

# Image scaling

Scale interlaced and planar images.

## Topics

### Planar Image Scaling

func vImageScale_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales an 8-bit planar image to fit a destination buffer.

func vImageScale_Planar16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales an unsigned 16-bit planar image to fit a destination buffer.

func vImageScale_Planar16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales a signed 16-bit planar image to fit a destination buffer.

func vImageScale_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales a floating-point 16-bit planar image to fit a destination buffer.

func vImageScale_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales a 32-bit planar image to fit a destination buffer.

### Interleaved Image Scaling

func vImageScale_CbCr8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales an 8-bit-per-channel, 2-channel interleaved image to fit a destination buffer.

func vImageScale_CbCr16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales an unsigned 16-bit-per-channel, 2-channel interleaved image to fit a destination buffer.

func vImageScale_CbCr16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales a floating-point 16-bit-per-channel, 2-channel interleaved image to fit a destination buffer.

func vImageScale_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales an 8-bit-per-channel, 4-channel interleaved image to fit a destination buffer.

func vImageScale_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales an unsigned 16-bit-per-channel, 4-channel interleaved image to fit a destination buffer.

func vImageScale_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales a signed 16-bit-per-channel, 4-channel interleaved image to fit a destination buffer.

func vImageScale_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales a floating-point 16-bit-per-channel, 4-channel interleaved image to fit a destination buffer.

func vImageScale_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales a 32-bit-per-channel, 4-channel interleaved image to fit a destination buffer.

func vImageScale_XRGB2101010W(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_Flags) -> vImage_Error

Scales a 2-bit alpha, 10-bit RGB interleaved image to fit a destination buffer.

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

Image rotation

Rotate images by arbitrary angles or by multiples of 90 degrees.

Getting the Buffer Size

Calculate the size of the temporary buffer needed by a high-level geometry functions.

