

- Accelerate
- vImage
- vImage Operations
-  Permuting Channels 

API Collection

# Permuting Channels

Reorder the channels in an image.

## Topics

### Permuting channels

func vImagePermuteChannels_RGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Permutes the channels of an 8-bit-per-channel, 3-channel interleaved buffer.

func vImagePermuteChannels_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Permutes the channels of an 8-bit-per-channel, 4-channel interleaved buffer.

func vImagePermuteChannels_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Permutes the channels of an unsigned 16-bit-per-channel, 4-channel interleaved buffer.

func vImagePermuteChannels_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Permutes the channels of a floating-point 16-bit-per-channel, 4-channel interleaved buffer.

func vImagePermuteChannels_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Permutes the channels of a floating-point 32-bit-per-channel, 4-channel interleaved buffer.

### Permuting channels with masked insert

func vImagePermuteChannelsWithMaskedInsert_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, UInt8, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Permutes and overwrites the channels of an 8-bit-per-channel, 4-channel interleaved buffer.

func vImagePermuteChannelsWithMaskedInsert_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, UInt8, UnsafePointer&lt;UInt16>, vImage_Flags) -> vImage_Error

Permutes and overwrites the channels of an unsigned 16-bit-per-channel, 4-channel interleaved buffer.

func vImagePermuteChannelsWithMaskedInsert_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, UInt8, UnsafePointer&lt;Float>, vImage_Flags) -> vImage_Error

Permutes and overwrites the channels of a floating-point 32-bit-per-channel, 4-channel interleaved buffer.

