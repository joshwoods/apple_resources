

- Core Media
-  CMSampleBufferCreateCopyWithNewTiming(allocator:sampleBuffer:sampleTimingEntryCount:sampleTimingArray:sampleBufferOut:) 

Function

# CMSampleBufferCreateCopyWithNewTiming(allocator:sampleBuffer:sampleTimingEntryCount:sampleTimingArray:sampleBufferOut:)

Creates a copy of a sample buffer with new timing information.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferCreateCopyWithNewTiming(
    allocator: CFAllocator?,
    sampleBuffer originalSBuf: CMSampleBuffer,
    sampleTimingEntryCount numSampleTimingEntries: CMItemCount,
    sampleTimingArray: UnsafePointer?,
    sampleBufferOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

The allocator to use for allocating the `CMSampleBuffer` object. Pass `kCFAllocatorDefault` to use the default allocator.

`originalSBuf`  

`CMSampleBuffer` containing the original samples.

`numSampleTimingEntries`  

Number of entries in `sampleTimingArray`. Must be 0, 1, or the number of samples in `originalSBuf`.

`sampleTimingArray`  

Array of `CMSampleTimingInfo` structs, one struct per sample. If all samples have the same duration and are in presentation order, you can pass a single `CMSampleTimingInfo` struct with duration set to the duration of one sample, `presentationTimeStamp` set to the presentation time of the numerically earliest sample, and `decodeTimeStamp` set to `kCMTimeInvalid`. Behavior is undefined if samples in a `CMSampleBuffer` (or even in multiple buffers in the same stream) have the same `presentationTimeStamp`. Can be `NULL`.

`sampleBufferOut`  

On output, points to the newly created copy of `CMSampleBuffer`.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

This emulates `CMSampleBufferCreateCopy`, but changes the timing. The array parameters, `sampleTimingArray`, should have only one element if that same element applies to all samples.

All parameters are copied; on return, the caller can release them, free them, or reuse them. Any `outputPresentationTimestamp` that has been set on the original buffer isn’t copied because it’s no longer relevant. On return, the caller owns the returned `CMSampleBuffer`, and must release it when done with it.

## See Also

### Copying Sample Buffers

func CMSampleBufferCreateCopy(allocator: CFAllocator?, sampleBuffer: CMSampleBuffer, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a copy of a sample buffer.

func CMSampleBufferCopySampleBufferForRange(allocator: CFAllocator?, sampleBuffer: CMSampleBuffer, sampleRange: CFRange, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer that contains a range of samples from an existing sample buffer.

