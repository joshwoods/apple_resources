

- Core Media
-  CMSampleBufferSetDataBuffer(\_:newValue:) 

Function

# CMSampleBufferSetDataBuffer(\_:newValue:)

Sets a block buffer of media data on a sample buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferSetDataBuffer(
    _ sbuf: CMSampleBuffer,
    newValue dataBuffer: CMBlockBuffer
) -> OSStatus
```

## Parameters 

`sbuf`  

The sample buffer being modified.

`dataBuffer`  

`CMBlockBuffer` of data being associated with.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

If successful, this operation retains the `dataBuffer`. This allows the caller to release the `dataBuffer` after calling this API, if it has no further need to reference it. This is a write-once operation; it fails if the `CMSampleBuffer` already has a `dataBuffer`. This API allows a `CMSampleBuffer` to exist, with timing and format information, before the associated data shows up.Example of usage: Some media services may have access to sample size, timing, and format information before the data is read. Such services may create `CMSampleBuffers` with that information and insert them into queues early, and use this API to attach the `CMBlockBuffers` later, when the data becomes ready.

## See Also

### Modifying Sample Buffers

func CMSampleBufferGetDataBuffer(CMSampleBuffer) -> CMBlockBuffer?

Returns a block buffer that contains the media data.

func CMSampleBufferGetImageBuffer(CMSampleBuffer) -> CVImageBuffer?

Returns an image buffer that contains the media data.

func CMSampleBufferGetAudioBufferListWithRetainedBlockBuffer(CMSampleBuffer, bufferListSizeNeededOut: UnsafeMutablePointer&lt;Int>?, bufferListOut: UnsafeMutablePointer&lt;AudioBufferList>?, bufferListSize: Int, blockBufferAllocator: CFAllocator?, blockBufferMemoryAllocator: CFAllocator?, flags: UInt32, blockBufferOut: UnsafeMutablePointer&lt;CMBlockBuffer?>?) -> OSStatus

Returns an audio buffer list that contains the media data.

func CMSampleBufferSetDataBufferFromAudioBufferList(CMSampleBuffer, blockBufferAllocator: CFAllocator?, blockBufferMemoryAllocator: CFAllocator?, flags: UInt32, bufferList: UnsafePointer&lt;AudioBufferList>) -> OSStatus

Creates a block buffer that contains a copy of the data from an audio buffer list.

func CMSampleBufferCopyPCMDataIntoAudioBufferList(CMSampleBuffer, at: Int32, frameCount: Int32, into: UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Copies PCM audio data from a sample buffer into an audio buffer list.

func CMSampleBufferGetAudioStreamPacketDescriptions(CMSampleBuffer, allocatedSize: Int, packetDescriptionsOut: UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, packetDescriptionsSizeNeededOut: UnsafeMutablePointer&lt;Int>?) -> OSStatus

Creates an array of audio stream packet descriptions.

func CMSampleBufferGetAudioStreamPacketDescriptionsPtr(CMSampleBuffer, packetDescriptionsPointerOut: UnsafeMutablePointer&lt;UnsafePointer&lt;AudioStreamPacketDescription>?>?, sizeOut: UnsafeMutablePointer&lt;Int>?) -> OSStatus

Returns a pointer to a constant array of audio stream packet descriptions.

