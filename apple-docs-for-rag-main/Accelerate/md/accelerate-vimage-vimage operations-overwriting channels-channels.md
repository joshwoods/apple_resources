

- Accelerate
- vImage
- vImage Operations
-  Overwriting channels 

API Collection

# Overwriting channels

Overwrite the channels of a buffer.

## Topics

### Overwriting with another buffer

func vImageSelectChannels_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, vImage_Flags) -> vImage_Error

Overwrites the channels of an 8-bit-per-channel, 4-channel interleaved buffer with the specified channels of the corresponding pixels of a second buffer.

func vImageSelectChannels_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, vImage_Flags) -> vImage_Error

Overwrites the channels of a floating-point 32-bit-per-channel, 4-channel interleaved buffer with the specified channels of the corresponding pixels of a second buffer.

func vImageOverwriteChannels_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, vImage_Flags) -> vImage_Error

Overwrites the channels of an 8-bit-per-channel, 4-channel interleaved buffer with the corresponding pixels of a planar buffer.

func vImageOverwriteChannels_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, vImage_Flags) -> vImage_Error

Overwrites the channels of a floating-point 32-bit-per-channel, 4-channel interleaved buffer with the corresponding pixels of a planar buffer.

### Overwriting with pixel values

func vImageOverwriteChannelsWithPixel_ARGB8888(UnsafePointer&lt;UInt8>!, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, vImage_Flags) -> vImage_Error

Overwrites the channels of an 8-bit-per-channel, 4-channel interleaved buffer with the specified channels of a pixel value.

func vImageOverwriteChannelsWithPixel_ARGB16U(UnsafePointer&lt;UInt16>!, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, vImage_Flags) -> vImage_Error

Overwrites the channels of an unsigned 16-bit-per-channel, 4-channel interleaved buffer with the specified channels of a pixel value.

func vImageOverwriteChannelsWithPixel_ARGBFFFF(UnsafePointer&lt;Float>!, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, vImage_Flags) -> vImage_Error

Overwrites the channels of a floating-point 32-bit-per-channel, 4-channel interleaved buffer with the specified channels of a pixel value.

### Overwriting with scalar values

func vImageOverwriteChannelsWithScalar_Planar8(Pixel_8, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Overwrites an 8-bit planar buffer with the specified scalar value in place.

func vImageOverwriteChannelsWithScalar_Planar16U(Pixel_16U, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Overwrites an unsigned 16-bit planar buffer with the specified scalar value in place.

func vImageOverwriteChannelsWithScalar_Planar16S(Pixel_16S, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Overwrites a signed 16-bit planar buffer with the specified scalar value in place.

func vImageOverwriteChannelsWithScalar_Planar16F(Pixel_16F, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Overwrites a floating-point 16-bit planar buffer with the specified scalar value in place.

func vImageOverwriteChannelsWithScalar_PlanarF(Pixel_F, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Overwrites a floating-point 32-bit planar buffer with the specified scalar value in place.

func vImageOverwriteChannelsWithScalar_ARGB8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, vImage_Flags) -> vImage_Error

Overwrites the selected channels of an 8-bit-per-channel, 4-channel interleaved buffer with the specified scalar value.

func vImageOverwriteChannelsWithScalar_ARGBFFFF(Pixel_F, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, vImage_Flags) -> vImage_Error

Overwrites the selected channels of a 32-bit-per-channel, 4-channel interleaved buffer with the specified scalar value.

