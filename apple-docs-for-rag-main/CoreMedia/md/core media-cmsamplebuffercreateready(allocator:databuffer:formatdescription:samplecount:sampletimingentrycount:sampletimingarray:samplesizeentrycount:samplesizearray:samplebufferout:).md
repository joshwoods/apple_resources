

- Core Media
-  CMSampleBufferCreateReady(allocator:dataBuffer:formatDescription:sampleCount:sampleTimingEntryCount:sampleTimingArray:sampleSizeEntryCount:sampleSizeArray:sampleBufferOut:) 

Function

# CMSampleBufferCreateReady(allocator:dataBuffer:formatDescription:sampleCount:sampleTimingEntryCount:sampleTimingArray:sampleSizeEntryCount:sampleSizeArray:sampleBufferOut:)

Creates a sample buffer with media data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferCreateReady(
    allocator: CFAllocator?,
    dataBuffer: CMBlockBuffer?,
    formatDescription: CMFormatDescription?,
    sampleCount numSamples: CMItemCount,
    sampleTimingEntryCount numSampleTimingEntries: CMItemCount,
    sampleTimingArray: UnsafePointer?,
    sampleSizeEntryCount numSampleSizeEntries: CMItemCount,
    sampleSizeArray: UnsafePointer?,
    sampleBufferOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

The allocator to use for allocating the `CMSampleBuffer` object. Pass `kCFAllocatorDefault` to use the default allocator.

`dataBuffer`  

`CMBlockBuffer` that already contains the media data. Must not be `NULL`.

`formatDescription`  

A description of the media data’s format. Can be `NULL`.

`numSamples`  

Number of samples in the `CMSampleBuffer`. Can be 0.

`numSampleTimingEntries`  

Number of entries in sampleTimingArray. Must be 0, 1, or `numSamples`.

`sampleTimingArray`  

Array of `CMSampleTimingInfo` structs, one struct per sample. If all samples have the same duration and are in presentation order, you can pass a single `CMSampleTimingInfo` struct with duration set to the duration of one sample, `presentationTimeStamp` set to the presentation time of the numerically earliest sample, and `decodeTimeStamp` set to `kCMTimeInvalid`. The behavior is undefined if samples in a `CMSampleBuffer` (or even in multiple buffers in the same stream) have the same `presentationTimeStamp`. Can be `NULL`.

`numSampleSizeEntries`  

Number of entries in `sampleSizeArray`. Must be 0, 1, or `numSamples`.

`sampleSizeArray`  

Array of size entries, one entry per sample. If all samples have the same size, you can pass a single size entry containing the size of one sample. Can be `NULL`.

Must be `NULL` if the samples are non-contiguous in the buffer (eg. non-interleaved audio, where the channel values for a single sample are scattered through the buffer).

`sampleBufferOut`  

Returned newly created `CMSampleBuffer`.

## Discussion

This function is identical to CMSampleBufferCreate(allocator:dataBuffer:dataReady:makeDataReadyCallback:refcon:formatDescription:sampleCount:sampleTimingEntryCount:sampleTimingArray:sampleSizeEntryCount:sampleSizeArray:sampleBufferOut:) except that `dataReady` is always `true`, and so no `makeDataReadyCallback` or `refcon` needs to be passed.

## See Also

### Creating Sample Buffers

func CMSampleBufferCreateReadyWithImageBuffer(allocator: CFAllocator?, imageBuffer: CVImageBuffer, formatDescription: CMVideoFormatDescription, sampleTiming: UnsafePointer&lt;CMSampleTimingInfo>, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer with image data.

func CMAudioSampleBufferCreateReadyWithPacketDescriptions(allocator: CFAllocator?, dataBuffer: CMBlockBuffer, formatDescription: CMFormatDescription, sampleCount: CMItemCount, presentationTimeStamp: CMTime, packetDescriptions: UnsafePointer&lt;AudioStreamPacketDescription>?, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer with packet descriptions.

func CMSampleBufferCreateWithMakeDataReadyHandler(CFAllocator?, CMBlockBuffer?, Bool, CMFormatDescription?, CMItemCount, CMItemCount, UnsafePointer&lt;CMSampleTimingInfo>?, CMItemCount, UnsafePointer&lt;Int>?, UnsafeMutablePointer&lt;CMSampleBuffer?>, CMSampleBufferMakeDataReadyHandler?) -> OSStatus

Creates a sample buffer with a handler to make the data ready for use.

func CMSampleBufferCreateForImageBufferWithMakeDataReadyHandler(CFAllocator?, CVImageBuffer, Bool, CMVideoFormatDescription, UnsafePointer&lt;CMSampleTimingInfo>, UnsafeMutablePointer&lt;CMSampleBuffer?>, CMSampleBufferMakeDataReadyHandler?) -> OSStatus

Creates a sample buffer with an image buffer and a handler to make the data ready for use.

func CMAudioSampleBufferCreateWithPacketDescriptionsAndMakeDataReadyHandler(CFAllocator?, CMBlockBuffer?, Bool, CMFormatDescription, CMItemCount, CMTime, UnsafePointer&lt;AudioStreamPacketDescription>?, UnsafeMutablePointer&lt;CMSampleBuffer?>, CMSampleBufferMakeDataReadyHandler?) -> OSStatus

Creates a sample buffer with packet descriptions and a handler to make the data ready for use.

func CMSampleBufferCreate(allocator: CFAllocator?, dataBuffer: CMBlockBuffer?, dataReady: Bool, makeDataReadyCallback: CMSampleBufferMakeDataReadyCallback?, refcon: UnsafeMutableRawPointer?, formatDescription: CMFormatDescription?, sampleCount: CMItemCount, sampleTimingEntryCount: CMItemCount, sampleTimingArray: UnsafePointer&lt;CMSampleTimingInfo>?, sampleSizeEntryCount: CMItemCount, sampleSizeArray: UnsafePointer&lt;Int>?, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer with a callback to make the data ready for use.

func CMSampleBufferCreateForImageBuffer(allocator: CFAllocator?, imageBuffer: CVImageBuffer, dataReady: Bool, makeDataReadyCallback: CMSampleBufferMakeDataReadyCallback?, refcon: UnsafeMutableRawPointer?, formatDescription: CMVideoFormatDescription, sampleTiming: UnsafePointer&lt;CMSampleTimingInfo>, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer with an image buffer and a callback to make the data ready for use.

func CMAudioSampleBufferCreateWithPacketDescriptions(allocator: CFAllocator?, dataBuffer: CMBlockBuffer?, dataReady: Bool, makeDataReadyCallback: CMSampleBufferMakeDataReadyCallback?, refcon: UnsafeMutableRawPointer?, formatDescription: CMFormatDescription, sampleCount: CMItemCount, presentationTimeStamp: CMTime, packetDescriptions: UnsafePointer&lt;AudioStreamPacketDescription>?, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer with packet descriptions and a callback to make the data ready for use.

