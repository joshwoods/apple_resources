

- Core Media
-  CMSampleBufferCreateCopy(allocator:sampleBuffer:sampleBufferOut:) 

Function

# CMSampleBufferCreateCopy(allocator:sampleBuffer:sampleBufferOut:)

Creates a copy of a sample buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferCreateCopy(
    allocator: CFAllocator?,
    sampleBuffer sbuf: CMSampleBuffer,
    sampleBufferOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

The allocator to use for allocating the `CMSampleBuffer` object. Pass `kCFAllocatorDefault` to use the default allocator.

`sbuf`  

`CMSampleBuffer` being copied.

`sampleBufferOut`  

On output, points to the newly created copy of `CMSampleBuffer`.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

The copy is shallow: scalar properties (sizes and timing) are copied directly, the data buffer and format description are retained, and the attachments that can be propagated are retained by the copy’s dictionary. If `sbuf’s` data isn’t ready, the copy will be set to track its readiness.

## See Also

### Copying Sample Buffers

func CMSampleBufferCreateCopyWithNewTiming(allocator: CFAllocator?, sampleBuffer: CMSampleBuffer, sampleTimingEntryCount: CMItemCount, sampleTimingArray: UnsafePointer&lt;CMSampleTimingInfo>?, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a copy of a sample buffer with new timing information.

func CMSampleBufferCopySampleBufferForRange(allocator: CFAllocator?, sampleBuffer: CMSampleBuffer, sampleRange: CFRange, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer that contains a range of samples from an existing sample buffer.

