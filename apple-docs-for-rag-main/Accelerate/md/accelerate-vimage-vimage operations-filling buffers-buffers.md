

- Accelerate
- vImage
- vImage Operations
-  Filling buffers 

API Collection

# Filling buffers

Fill a buffer with a specified color.

## Topics

### Filling buffers

func vImageBufferFill_CbCr8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Fills an 8-bit-per-channel, 2-channel interleaved buffer with a specified color.

func vImageBufferFill_CbCr16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt16>, vImage_Flags) -> vImage_Error

Fills an unsigned 16-bit-per-channel, 2-channel interleaved buffer with a specified color.

func vImageBufferFill_CbCr16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Int16>, vImage_Flags) -> vImage_Error

func vImageBufferFill_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Fills an 8-bit-per-channel, 4-channel interleaved buffer with a specified color.

func vImageBufferFill_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt16>, vImage_Flags) -> vImage_Error

Fills an unsigned 16-bit-per-channel, 4-channel interleaved buffer with a specified color.

func vImageBufferFill_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Int16>, vImage_Flags) -> vImage_Error

Fills a signed 16-bit-per-channel, 4-channel interleaved buffer with a specified color.

func vImageBufferFill_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt16>, vImage_Flags) -> vImage_Error

Fills a floating-point 16-bit-per-channel, 4-channel interleaved buffer with a specified color.

func vImageBufferFill_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, vImage_Flags) -> vImage_Error

Fills a floating-point 32-bit-per-channel, 4-channel interleaved buffer with a specified color.

