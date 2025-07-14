

- Accelerate
-  vImageBufferFill_CbCr16S(\_:\_:\_:) 

Function

# vImageBufferFill_CbCr16S(\_:\_:\_:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func vImageBufferFill_CbCr16S(
    _ dest: UnsafePointer,
    _ color: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`dest`  

A pointer to a valid and initialized vImage_Buffer struct, that points to a buffer containing destination pixels.

`color`  

A pixel value to fill the destination buffer.

`flags`  

\P kvImageNoFlags Default operation \p kvImageDoNotTile Disable internal multithreading.

## Return Value

kvImageNoError Success

## See Also

### Filling buffers

func vImageBufferFill_CbCr8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Fills an 8-bit-per-channel, 2-channel interleaved buffer with a specified color.

func vImageBufferFill_CbCr16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt16>, vImage_Flags) -> vImage_Error

Fills an unsigned 16-bit-per-channel, 2-channel interleaved buffer with a specified color.

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

