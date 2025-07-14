

- Core Media
-  CMSampleBufferCopySampleBufferForRange(allocator:sampleBuffer:sampleRange:sampleBufferOut:) 

Function

# CMSampleBufferCopySampleBufferForRange(allocator:sampleBuffer:sampleRange:sampleBufferOut:)

Creates a sample buffer that contains a range of samples from an existing sample buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferCopySampleBufferForRange(
    allocator: CFAllocator?,
    sampleBuffer sbuf: CMSampleBuffer,
    sampleRange: CFRange,
    sampleBufferOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

The allocator to use for allocating the `CMSampleBuffer` object. Pass `kCFAllocatorDefault` to use the default allocator.

`sbuf`  

The sample buffer containing the original samples.

`sampleRange`  

The range of samples to copy from `sbuf`, where sample 0 is the first sample in the `sbuf`.\`\`

`sampleBufferOut`  

On output, points to the newly created `CMSampleBuffer`.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

Note

Samples containing non-interleaved audio aren’t supported.

## See Also

### Copying Sample Buffers

func CMSampleBufferCreateCopy(allocator: CFAllocator?, sampleBuffer: CMSampleBuffer, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a copy of a sample buffer.

func CMSampleBufferCreateCopyWithNewTiming(allocator: CFAllocator?, sampleBuffer: CMSampleBuffer, sampleTimingEntryCount: CMItemCount, sampleTimingArray: UnsafePointer&lt;CMSampleTimingInfo>?, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a copy of a sample buffer with new timing information.

