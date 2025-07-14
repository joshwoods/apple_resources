

- Core Media
-  CMSampleBufferSetDataBufferFromAudioBufferList(\_:blockBufferAllocator:blockBufferMemoryAllocator:flags:bufferList:) 

Function

# CMSampleBufferSetDataBufferFromAudioBufferList(\_:blockBufferAllocator:blockBufferMemoryAllocator:flags:bufferList:)

Creates a block buffer that contains a copy of the data from an audio buffer list.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferSetDataBufferFromAudioBufferList(
    _ sbuf: CMSampleBuffer,
    blockBufferAllocator blockBufferStructureAllocator: CFAllocator?,
    blockBufferMemoryAllocator blockBufferBlockAllocator: CFAllocator?,
    flags: UInt32,
    bufferList: UnsafePointer
) -> OSStatus
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being modified.

`blockBufferStructureAllocator`  

Allocator to use when creating the `CMBlockBuffer` structure.

`blockBufferBlockAllocator`  

Allocator to use for memory block held by the `CMBlockBuffer`.

`flags`  

Flags controlling operation.

`bufferList`  

Buffer list whose data will be copied into the new `CMBlockBuffer`.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

Creates a `CMBlockBuffer` containing a copy of the data from the `AudioBufferList`, and sets that as the sample buffer’s data buffer. The resulting buffer(s) in the sample buffer will be 16-byte-aligned if `kCMSampleBufferFlag_AudioBufferList_Assure16ByteAlignment` is passed in.

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

func CMSampleBufferCopyPCMDataIntoAudioBufferList(CMSampleBuffer, at: Int32, frameCount: Int32, into: UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Copies PCM audio data from a sample buffer into an audio buffer list.

func CMSampleBufferGetAudioStreamPacketDescriptions(CMSampleBuffer, allocatedSize: Int, packetDescriptionsOut: UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, packetDescriptionsSizeNeededOut: UnsafeMutablePointer&lt;Int>?) -> OSStatus

Creates an array of audio stream packet descriptions.

func CMSampleBufferGetAudioStreamPacketDescriptionsPtr(CMSampleBuffer, packetDescriptionsPointerOut: UnsafeMutablePointer&lt;UnsafePointer&lt;AudioStreamPacketDescription>?>?, sizeOut: UnsafeMutablePointer&lt;Int>?) -> OSStatus

Returns a pointer to a constant array of audio stream packet descriptions.

