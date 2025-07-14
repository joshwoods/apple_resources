

- Core Media
-  CMSampleBufferGetAudioStreamPacketDescriptions(\_:allocatedSize:packetDescriptionsOut:packetDescriptionsSizeNeededOut:) 

Function

# CMSampleBufferGetAudioStreamPacketDescriptions(\_:allocatedSize:packetDescriptionsOut:packetDescriptionsSizeNeededOut:)

Creates an array of audio stream packet descriptions.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferGetAudioStreamPacketDescriptions(
    _ sbuf: CMSampleBuffer,
    allocatedSize packetDescriptionsSize: Int,
    packetDescriptionsOut: UnsafeMutablePointer?,
    packetDescriptionsSizeNeededOut: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`sbuf`  

`CMSampleBuffer` being accessed.

`packetDescriptionsSize`  

Size of `packetDescriptionsOut` as allocated by the caller.

`packetDescriptionsOut`  

Allocated by the caller, receives the packet descriptions for the samples in the `CMSampleBuffer`. If non-`NULL` and `packetDescriptionsSize` is too small, `kFigSampleBufferError_ArrayTooSmall` is returned.

`packetDescriptionsSizeNeededOut`  

Used to query for the correct size required for `packetDescriptionsOut`. May be `NULL`.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

Creates an array of `AudioStreamPacketDescriptions` for the variable bytes per packet or variable frames per packet audio data in the provided `CMSampleBuffer`. Constant bit rate, constant frames-per-packet audio yields a return value of `noErr` and no packet descriptions.

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

func CMSampleBufferGetAudioStreamPacketDescriptionsPtr(CMSampleBuffer, packetDescriptionsPointerOut: UnsafeMutablePointer&lt;UnsafePointer&lt;AudioStreamPacketDescription>?>?, sizeOut: UnsafeMutablePointer&lt;Int>?) -> OSStatus

Returns a pointer to a constant array of audio stream packet descriptions.

