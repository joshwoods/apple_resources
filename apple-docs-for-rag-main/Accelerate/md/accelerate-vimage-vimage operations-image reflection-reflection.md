

- Accelerate
- vImage
- vImage Operations
-  Image reflection 

API Collection

# Image reflection

Reflect images horizontally and vertically.

## Topics

### Applying horizontal reflection to 8-bit-per-channel buffers

func vImageHorizontalReflect_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects an 8-bit planar image horizontally across the center vertical line.

func vImageHorizontalReflect_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects an 8-bit-per-channel, 4-channel interleaved image horizontally across the center vertical line.

### Applying horizontal reflection to 16-bit-per-channel buffers

func vImageHorizontalReflect_Planar16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects an unsigned 16-bit planar image horizontally across the center vertical line.

func vImageHorizontalReflect_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a floating-point 16-bit planar image horizontally across the center vertical line.

func vImageHorizontalReflect_CbCr16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a floating-point 16-bit-per-channel, 2-channel interleaved image horizontally across the center vertical line.

func vImageHorizontalReflect_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects an unsigned 16-bit-per-channel, 4-channel interleaved image horizontally across the center vertical line.

func vImageHorizontalReflect_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a signed 16-bit-per-channel, 4-channel interleaved image horizontally across the center vertical line.

func vImageHorizontalReflect_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a floating-point 16-bit-per-channel, 4-channel interleaved image horizontally across the center vertical line.

### Applying horizontal reflection to 32-bit-per-channel buffers

func vImageHorizontalReflect_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a 32-bit planar image horizontally across the center vertical line.

func vImageHorizontalReflect_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a 32-bit-per-channel, 4-channel interleaved image horizontally across the center vertical line.

### Applying vertical reflection to 8-bit-per-channel buffers

func vImageVerticalReflect_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects an 8-bit planar image vertically across the center horizontal line.

func vImageVerticalReflect_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects an 8-bit-per-channel, 4-channel interleaved image vertically across the center horizontal line.

### Applying vertical reflection to 16-bit-per-channel buffers

func vImageVerticalReflect_Planar16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects an unsigned 16-bit planar image vertically across the center horizontal line.

func vImageVerticalReflect_Planar16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a floating-point 16-bit planar image vertically across the center horizontal line.

func vImageVerticalReflect_CbCr16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a floating-point 16-bit-per-channel, 2-channel interleaved image vertically across the center horizontal line.

func vImageVerticalReflect_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects an unsigned 16-bit-per-channel, 4-channel interleaved image vertically across the center horizontal line.

func vImageVerticalReflect_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a signed 16-bit-per-channel, 4-channel interleaved image vertically across the center horizontal line.

func vImageVerticalReflect_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a floating-point 16-bit-per-channel, 4-channel interleaved image vertically across the center horizontal line.

### Applying vertical reflection to 32-bit-per-channel buffers

func vImageVerticalReflect_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a 32-bit planar image vertically across the center horizontal line.

func vImageVerticalReflect_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Reflects a 32-bit-per-channel, 4-channel interleaved image vertically across the center horizontal line.

## See Also

### Applying geometric transforms to image buffers

Resampling in vImage

Learn how vImage resamples image data during geometric operations.

Applying affine transformations to images

Translate, rotate, and scale images.

Applying projective transformations to images

Warp images in three dimensions.

Image shearing

Shear images horizontally and vertically.

Image rotation

Rotate images by arbitrary angles or by multiples of 90 degrees.

Image scaling

Scale interlaced and planar images.

Getting the Buffer Size

Calculate the size of the temporary buffer needed by a high-level geometry functions.

