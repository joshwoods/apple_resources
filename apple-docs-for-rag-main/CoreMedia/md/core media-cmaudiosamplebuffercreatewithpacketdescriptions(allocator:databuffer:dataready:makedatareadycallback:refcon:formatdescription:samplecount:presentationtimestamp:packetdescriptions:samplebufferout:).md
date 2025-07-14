

- Core Media
-  CMAudioSampleBufferCreateWithPacketDescriptions(allocator:dataBuffer:dataReady:makeDataReadyCallback:refcon:formatDescription:sampleCount:presentationTimeStamp:packetDescriptions:sampleBufferOut:) 

Function

# CMAudioSampleBufferCreateWithPacketDescriptions(allocator:dataBuffer:dataReady:makeDataReadyCallback:refcon:formatDescription:sampleCount:presentationTimeStamp:packetDescriptions:sampleBufferOut:)

Creates a sample buffer with packet descriptions and a callback to make the data ready for use.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMAudioSampleBufferCreateWithPacketDescriptions(
    allocator: CFAllocator?,
    dataBuffer: CMBlockBuffer?,
    dataReady: Bool,
    makeDataReadyCallback: CMSampleBufferMakeDataReadyCallback?,
    refcon makeDataReadyRefcon: UnsafeMutableRawPointer?,
    formatDescription: CMFormatDescription,
    sampleCount numSamples: CMItemCount,
    presentationTimeStamp: CMTime,
    packetDescriptions: UnsafePointer?,
    sampleBufferOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

The allocator to use for allocating the `CMSampleBuffer` object. Pass `kCFAllocatorDefault` to use the default allocator.

`dataBuffer`  

`CMBlockBuffer` for the media data. This can be `NULL`, a `CMBlockBuffer` with no backing memory, a `CMBlockBuffer` with backing memory but no data yet, or a `CMBlockBuffer` that already contains the media data. If `CMBlockBuffer` contains the media data, `dataReady` should be `true`.

`dataReady`  

Indicates whether or not the `BlockBuffer` already contains the media data.

`makeDataReadyCallback`  

Callback that `CMSampleBufferMakeDataReady` should call to make the data ready. Can be `NULL`.

`makeDataReadyRefcon`  

The reference constant, CMSampleBufferMakeDataReady(_:), that this function should pass to the callback.

`formatDescription`  

A description of the media data’s format. Can’t be `NULL`.

`numSamples`  

Number of samples in the `CMSampleBuffer`. Must not be 0.

`presentationTimeStamp`  

Timestamp of the first sample in the buffer. Must be a numeric `CMTime`.

`packetDescriptions`  

Array of `packetDescriptions`, one for each of `numSamples`. May be `NULL` if the samples are known to have a constant number of frames per packet and a constant size.

`sampleBufferOut`  

On output, points to the newly created `CMSampleBuffer`.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

Provides an optimization over `CMSampleBufferCreate`() when the caller already has `packetDescriptions` for the audio data. This routine uses the packetDescriptions to create the sizing and timing arrays required to make the sample buffer if necessary.

## Topics

### Callbacks

typealias CMSampleBufferMakeDataReadyCallback

Client callback called by CMSampleBufferMakeDataReady(_:).

## See Also

### Creating Sample Buffers

func CMSampleBufferCreateReady(allocator: CFAllocator?, dataBuffer: CMBlockBuffer?, formatDescription: CMFormatDescription?, sampleCount: CMItemCount, sampleTimingEntryCount: CMItemCount, sampleTimingArray: UnsafePointer&lt;CMSampleTimingInfo>?, sampleSizeEntryCount: CMItemCount, sampleSizeArray: UnsafePointer&lt;Int>?, sampleBufferOut: UnsafeMutablePointer&lt;CMSampleBuffer?>) -> OSStatus

Creates a sample buffer with media data.

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

