

- Core Media
-  CMSampleBufferCopyPCMDataIntoAudioBufferList(\_:at:frameCount:into:) 

Function

# CMSampleBufferCopyPCMDataIntoAudioBufferList(\_:at:frameCount:into:)

Copies PCM audio data from a sample buffer into an audio buffer list.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferCopyPCMDataIntoAudioBufferList(
    _ sbuf: CMSampleBuffer,
    at frameOffset: Int32,
    frameCount numFrames: Int32,
    into bufferList: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`sbuf`  

The sample buffer containing the PCM audio data to be copied.

`frameOffset`  

The frame offset number from which to begin the copy.

`numFrames`  

The total number of frames to copy.

`bufferList`  

The audio buffer list to populate.

## Discussion

The AudioBufferList must contain the same number of channels and its data buffers must be sized to hold the specified number of frames.

This API is specific to audio format sample buffers, and will return `kCMSampleBufferError_InvalidMediaTypeForOperation` if called with a non-audio sample buffer. It will return an error if the sample buffer doesn’t contain PCM audio data or if its data buffer isn’t ready.

## See Also

### Modifying Sample Buffers

func CMSampleBufferGetDataBuffer(CMSampleBuffer) -> CMBlockBuffer?

Returns a block buffer that contains the media data.

func CMSampleBufferSetDataBuffer(CMSampleBuffer, newValue: CMBlockBuffer) -> OSStatus

Sets a block buffer of media data on a sample buffer.

func CMSampleBufferGetImageBuffer(CMSampleBuffer) -> CVImageBuffer?

Returns an image buffer that contains the media data.

func CMSampleBufferGetAudioBufferListWithRetainedBlockBuffer(CMSampleBuffer, bufferListSizeNeededOut: UnsafeMutablePointer&lt;Int>?, bufferListOut: UnsafeMutablePointer&lt;AudioBufferList>?, bufferListSize: Int, blockBufferAllocator: CFAllocator?, blockBufferMemoryAllocator: CFAllocator?, flags: UInt32, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>?) -> OSStatus

Returns an audio buffer list that contains the media data.

func CMSampleBufferSetDataBufferFromAudioBufferList(CMSampleBuffer, blockBufferAllocator: CFAllocator?, blockBufferMemoryAllocator: CFAllocator?, flags: UInt32, bufferList: UnsafePointer&lt;AudioBufferList>) -> OSStatus

Creates a block buffer that contains a copy of the data from an audio buffer list.

func CMSampleBufferGetAudioStreamPacketDescriptions(CMSampleBuffer, allocatedSize: Int, packetDescriptionsOut: UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, packetDescriptionsSizeNeededOut: UnsafeMutablePointer&lt;Int>?) -> OSStatus

Creates an array of audio stream packet descriptions.

func CMSampleBufferGetAudioStreamPacketDescriptionsPtr(CMSampleBuffer, packetDescriptionsPointerOut: UnsafeMutablePointer&lt;UnsafePointer&lt;AudioStreamPacketDescription>?>?, sizeOut: UnsafeMutablePointer&lt;Int>?) -> OSStatus

Returns a pointer to a constant array of audio stream packet descriptions.

