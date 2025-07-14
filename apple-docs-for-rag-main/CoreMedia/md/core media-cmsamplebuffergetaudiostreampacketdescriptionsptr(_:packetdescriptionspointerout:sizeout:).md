

- Core Media
-  CMSampleBufferGetAudioStreamPacketDescriptionsPtr(\_:packetDescriptionsPointerOut:sizeOut:) 

Function

# CMSampleBufferGetAudioStreamPacketDescriptionsPtr(\_:packetDescriptionsPointerOut:sizeOut:)

Returns a pointer to a constant array of audio stream packet descriptions.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferGetAudioStreamPacketDescriptionsPtr(
    _ sbuf: CMSampleBuffer,
    packetDescriptionsPointerOut: UnsafeMutablePointer?>?,
    sizeOut packetDescriptionsSizeOut: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being modified.

`packetDescriptionsPointerOut`  

On output, contains pointer to a constant array of `AudioStreamPacketDescriptions`. May be `NULL`.

`packetDescriptionsSizeOut`  

Size in bytes of constant array of `AudioStreamPacketDescriptions`. May be `NULL`.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

Returns a pointer to (and size of) a constant array of `AudioStreamPacketDescriptions` for the variable bytes per packet or variable frames per packet audio data in the provided `CMSampleBuffer`. The pointer will remain valid as long as the buffer continues to be retained.

Constant bit rate, constant frames-per-packet audio yields a return value of `noErr` and no packet descriptions.

This API is specific to audio format sample buffers, and will return `kCMSampleBufferError_InvalidMediaTypeForOperation` if called with a non-audio sample buffer.

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

func CMSampleBufferCopyPCMDataIntoAudioBufferList(CMSampleBuffer, at: Int32, frameCount: Int32, into: UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Copies PCM audio data from a sample buffer into an audio buffer list.

func CMSampleBufferGetAudioStreamPacketDescriptions(CMSampleBuffer, allocatedSize: Int, packetDescriptionsOut: UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, packetDescriptionsSizeNeededOut: UnsafeMutablePointer&lt;Int>?) -> OSStatus

Creates an array of audio stream packet descriptions.

