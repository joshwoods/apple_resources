

- Accelerate
- vImage
- vImage Operations
-  Extracting channels 

API Collection

# Extracting channels

Extract one channel from a four-channel interleaved buffer.

## Topics

### Extracting channels

func vImageExtractChannel_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int, vImage_Flags) -> vImage_Error

Extracts a single channel from an 8-bit-per-channel, 4-channel interleaved buffer and writes the result to an 8-bit planar buffer.

func vImageExtractChannel_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int, vImage_Flags) -> vImage_Error

Extracts a single channel from an unsigned 16-bit-per-channel, 4-channel interleaved buffer and writes the result to an unsigned 16-bit planar buffer.

func vImageExtractChannel_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int, vImage_Flags) -> vImage_Error

Extracts a single channel from a 32-bit-per-channel, 4-channel interleaved buffer and writes the result to a 32-bit planar buffer.

