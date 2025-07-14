

- Accelerate
- vImage
- vImage Operations
-  Alpha compositing 

API Collection

# Alpha compositing

Composite images together.

## Topics

### Performing nonpremultiplied alpha compositing

func vImageAlphaBlend_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs nonpremultiplied alpha compositing of two 8-bit planar buffers.

func vImageAlphaBlend_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs nonpremultiplied alpha compositing of two 8-bit planar buffers.

func vImageAlphaBlend_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs nonpremultiplied alpha compositing of two 8-bit-per-channel, 4-channel ARGB buffers.

func vImageAlphaBlend_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs nonpremultiplied alpha compositing of two 32-bit-per-channel, 4-channel ARGB buffers.

### Performing premultiplied alpha compositing

func vImagePremultipliedAlphaBlend_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 8-bit planar buffers.

func vImagePremultipliedAlphaBlend_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 32-bit planar buffers.

func vImagePremultipliedAlphaBlend_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 8-bit-per-channel, 4-channel ARGB buffers.

func vImagePremultipliedAlphaBlend_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 32-bit-per-channel, 4-channel ARGB buffers.

func vImagePremultipliedAlphaBlend_BGRA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 8-bit-per-channel, 4-channel BGRA buffers.

vImagePremultipliedAlphaBlend_RGBA8888

Performs premultiplied alpha compositing of two 8-bit-per-channel, 4-channel RGBA buffers.

func vImagePremultipliedAlphaBlend_BGRAFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 32-bit-per-channel, 4-channel BGRA buffers.

vImagePremultipliedAlphaBlend_RGBAFFFF

Performs premultiplied alpha compositing of two 32-bit-per-channel, 4-channel RGBA buffers.

### Performing premultiplied alpha compositing with blend modes

func vImagePremultipliedAlphaBlendLighten_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs alpha compositing of two 8-bit-per-channel, 4-channel BGRA buffers using the lighten blend mode.

func vImagePremultipliedAlphaBlendDarken_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs alpha compositing of two 8-bit-per-channel, 4-channel BGRA buffers using the darken blend mode.

func vImagePremultipliedAlphaBlendScreen_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs alpha compositing of two 8-bit-per-channel, 4-channel BGRA buffers using the screen blend mode.

func vImagePremultipliedAlphaBlendMultiply_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs alpha compositing of two 8-bit-per-channel, 4-channel BGRA buffers using the multiply blend mode.

### Performing premultiplied alpha compositing with a permute

func vImagePremultipliedAlphaBlendWithPermute_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, Bool, vImage_Flags) -> vImage_Error

Permutes the top 8-bit, 4-channel premultiplied buffer, and composites with the bottom buffer.

func vImagePremultipliedAlphaBlendWithPermute_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, Bool, vImage_Flags) -> vImage_Error

Permutes the top 8-bit, 4-channel premultiplied buffer, and composites with the bottom buffer.

### Performing premultiplied alpha compositing with a single alpha value

func vImagePremultipliedConstAlphaBlend_Planar8(UnsafePointer&lt;vImage_Buffer>, Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 8-bit planar buffers and applies an extra alpha value to the top buffer.

func vImagePremultipliedConstAlphaBlend_PlanarF(UnsafePointer&lt;vImage_Buffer>, Pixel_F, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 32-bit planar buffers and applies an extra alpha value to the top buffer.

func vImagePremultipliedConstAlphaBlend_ARGB8888(UnsafePointer&lt;vImage_Buffer>, Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 8-bit-per-channel, 4-channel interleaved buffers and applies an extra alpha value to the top buffer.

func vImagePremultipliedConstAlphaBlend_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, Pixel_F, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Performs premultiplied alpha compositing of two 32-bit-per-channel, 4-channel interleaved buffers and applies an extra alpha value to the top buffer.

### Performing nonpremultiplied to premultiplied alpha compositing

func vImageAlphaBlend_NonpremultipliedToPremultiplied_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Composites a nonpremultiplied 8-bit planar buffer over a premultiplied 8-bit planar buffer and generates a premultiplied result.

func vImageAlphaBlend_NonpremultipliedToPremultiplied_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Composites a nonpremultiplied 32-bit planar buffer over a premultiplied 32-bit planar buffer and generates a premultiplied result.

func vImageAlphaBlend_NonpremultipliedToPremultiplied_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Composites a nonpremultiplied 8-bit-per-channel, ARGB buffer over a premultiplied ARGB buffer and generates a premultiplied result.

func vImageAlphaBlend_NonpremultipliedToPremultiplied_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Composites a nonpremultiplied 32-bit-per-channel, ARGB buffer over a premultiplied ARGB buffer and generates a premultiplied result.

### Converting from unpremultiplied to premultiplied format

func vImagePremultiplyData_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit planar buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a 32-bit planar buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit-per-channel, 4-channel ARGB buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit-per-channel, 4-channel RGBA buffer from nonpremultiplied alpha format to premultiplied alpha format.

vImagePremultiplyData_BGRA8888

Transforms an 8-bit-per-channel, 4-channel BGRA buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an unsigned 16-bit-per-channel, 4-channel ARGB buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_RGBA16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an unsigned 16-bit-per-channel, 4-channel RGBA buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_RGBA16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a floating-point 16-bit-per-channel, 4-channel RGBA buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_ARGB16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a fixed-point 16-bit-per-channel, 4-channel ARGB buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_RGBA16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a fixed-point 16-bit-per-channel, 4-channel RGBA buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a floating-point 32-bit-per-channel, 4-channel ARGB buffer from nonpremultiplied alpha format to premultiplied alpha format.

func vImagePremultiplyData_RGBAFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a floating-point 32-bit-per-channel, 4-channel ARGB buffer from nonpremultiplied alpha format to premultiplied alpha format.

vImagePremultiplyData_BGRAFFFF

Transforms a floating-point 32-bit-per-channel, 4-channel BGRA buffer from nonpremultiplied alpha format to premultiplied alpha format.

### Converting from premultiplied to unpremultiplied format

func vImageUnpremultiplyData_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit planar buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a 32-bit planar buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit-per-channel, 4-channel ARGB buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an 8-bit-per-channel, 4-channel RGBA buffer from premultiplied alpha format to nonpremultiplied alpha format.

vImageUnpremultiplyData_BGRA8888

Transforms an 8-bit-per-channel, 4-channel BGRA buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an unsigned 16-bit-per-channel, 4-channel ARGB buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_RGBA16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms an unsigned 16-bit-per-channel, 4-channel RGBA buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_RGBA16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a floating-point 16-bit-per-channel, 4-channel RGBA buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_ARGB16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a fixed-point 16-bit-per-channel, 4-channel ARGB buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_RGBA16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a fixed-point 16-bit-per-channel, 4-channel RGBA buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a 32-bit-per-channel, 4-channel ARGB buffer from premultiplied alpha format to nonpremultiplied alpha format.

func vImageUnpremultiplyData_RGBAFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Transforms a 32-bit-per-channel, 4-channel RGBA buffer from premultiplied alpha format to nonpremultiplied alpha format.

vImageUnpremultiplyData_BGRAFFFF

Transforms a 32-bit-per-channel, 4-channel BGRA buffer from premultiplied alpha format to nonpremultiplied alpha format.

### Clipping color values to alpha

func vImageClipToAlpha_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Clamps the values of an 8-bit planar buffer to the corresponding alpha values.

func vImageClipToAlpha_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Clamps the values of a 32-bit planar buffer to the corresponding alpha values.

func vImageClipToAlpha_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Clamps the values of an 8-bit-per-channel, 4-channel ARGB buffer to the corresponding alpha values.

func vImageClipToAlpha_RGBA8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Clamps the values of an 8-bit-per-channel, 4-channel RGBA buffer to the corresponding alpha values.

func vImageClipToAlpha_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Clamps the values of a 32-bit-per-channel, 4-channel ARGB buffer to the corresponding alpha values.

func vImageClipToAlpha_RGBAFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Clamps the values of a 32-bit-per-channel, 4-channel RGBA buffer to the corresponding alpha values.

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

Compositing images with vImage blend modes

Combine two images by using blend modes to create a single output.

