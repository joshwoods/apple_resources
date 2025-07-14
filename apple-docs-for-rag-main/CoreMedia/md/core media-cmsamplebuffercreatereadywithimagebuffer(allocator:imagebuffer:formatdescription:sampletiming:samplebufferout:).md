

- Core Media
-  CMSampleBufferCreateReadyWithImageBuffer(allocator:imageBuffer:formatDescription:sampleTiming:sampleBufferOut:) 

Function

# CMSampleBufferCreateReadyWithImageBuffer(allocator:imageBuffer:formatDescription:sampleTiming:sampleBufferOut:)

Creates a sample buffer with image data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferCreateReadyWithImageBuffer(
    allocator: CFAllocator?,
    imageBuffer: CVImageBuffer,
    formatDescription: CMVideoFormatDescription,
    sampleTiming: UnsafePointer,
    sampleBufferOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

The allocator to use for allocating the `CMSampleBuffer` object. Pass `kCFAllocatorDefault` to use the default allocator.

`imageBuffer`  

`CVImageBuffer` already containing the media data. Must not be `NULL`.

`formatDescription`  

A description of the media data’s format. See discussion below for constraints. May not be `NULL`.

`sampleTiming`  

A `CMSampleTimingInfo` struct that provides the timing information for the media represented by the `CVImageBuffer`.

`sampleBufferOut`  

Returned newly created `CMSampleBuffer`.

## Discussion

Unlike a `CMBlockBuffer`, which can reference many samples, a `CVImageBuffer` is defined to reference only one sample; therefore this routine has fewer parameters than `CMSampleBufferCreate`.

Sample timing information, which is a vector for `CMSampleBufferCreate`, consists of only one value for this routine.

The concept of sample size doesn’t apply to `CVImageBuffers`. As such, `CMSampleBufferGetSampleSizeArray` returns `kCMSampleBufferError_BufferHasNoSampleSizes`, and `CMSampleBufferGetSampleSize` returns 0.

Because `CVImageBuffers` hold visual data, the format description provided is a `CMVideoFormatDescription`. The format description must be consistent with the attributes and formatting information attached to the `CVImageBuffer`. The `width`, `height`, and `codecType` must match (for `CVPixelBuffers` the codec type is given by `CVPixelBufferGetPixelFormatType(pixelBuffer)`; for other `CVImageBuffers`, the `codecType` must be 0). The format description extensions must match the image buffer attachments for all the keys in the list returned by `CMVideoFormatDescriptionGetExtensionKeysCommonWithImageBuffers` (if absent in either they must be absent in both).

`CMSampleBufferCreateReadyWithImageBuffer` is identical to `CMSampleBufferCreateForImageBuffer` except that `dataReady` is always `true`, and so no `makeDataReadyCallback` or `refcon` needs to be passed.

## See Also

### Creating Sample Buffers

func CMSampleBufferCreateReady(allocator: CFAllocator?, dataBuffer: CMBlockBuffer?, formatDescription: CMFormatDescription?, sampleCount: CMItemCount, sampleTimingEntryCount: CMItemCount, sampleTimingArray: UnsafePointer&lt;CMSampleTimingInfo>?, sampleSizeEntryCount: CMItemCount, sampleSizeArray: UnsafePointer&lt;Int>?, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer with media data.

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

