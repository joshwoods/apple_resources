

- Accelerate
-  Morphology 

API Collection

# Morphology

Dilate and erode images.

## Topics

### Dilating an object

func vImageDilate_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;UInt8>, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Dilates an 8-bit planar buffer.

func vImageDilate_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Dilates a 32-bit planar buffer.

func vImageDilate_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;UInt8>, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Dilates an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageDilate_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Dilates a 32-bit-per-channel, 4-channel interleaved buffer.

### Eroding an object

func vImageErode_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;UInt8>, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Erodes an 8-bit planar buffer.

func vImageErode_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Erodes a 32-bit planar buffer.

func vImageErode_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;UInt8>, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Erodes an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageErode_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, vImagePixelCount, vImagePixelCount, UnsafePointer&lt;Float>, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Erodes a 32-bit-per-channel, 4-channel interleaved buffer.

### Maximizing an object

func vImageMax_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Maximizes an 8-bit planar buffer.

func vImageMax_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Maximizes a 32-bit planar buffer.

func vImageMax_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Maximizes an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageMax_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Maximizes a 32-bit-per-channel, 4-channel interleaved buffer.

### Minimizing an object

func vImageMin_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Minimizes an 8-bit planar buffer.

func vImageMin_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Minimizes a 32-bit planar buffer.

func vImageMin_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Minimizes an 8-bit-per-channel, 4-channel interleaved buffer.

func vImageMin_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImagePixelCount, vImage_Flags) -> vImage_Error

Minimizes an 8-bit-per-channel, 4-channel interleaved buffer.

## See Also

### Convolution and Morphology

Blurring an image

Filter an image by convolving it with custom and high-speed kernels.

Adding a bokeh effect to images

Simulate a bokeh effect by applying dilation.

Convolution

Apply a convolution kernel to an image.

