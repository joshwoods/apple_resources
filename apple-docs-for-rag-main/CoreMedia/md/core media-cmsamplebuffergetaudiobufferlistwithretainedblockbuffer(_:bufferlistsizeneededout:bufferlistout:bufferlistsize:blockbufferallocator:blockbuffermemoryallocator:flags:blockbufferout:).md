

- Core Media
-  CMSampleBufferGetAudioBufferListWithRetainedBlockBuffer(\_:bufferListSizeNeededOut:bufferListOut:bufferListSize:blockBufferAllocator:blockBufferMemoryAllocator:flags:blockBufferOut:) 

Function

# CMSampleBufferGetAudioBufferListWithRetainedBlockBuffer(\_:bufferListSizeNeededOut:bufferListOut:bufferListSize:blockBufferAllocator:blockBufferMemoryAllocator:flags:blockBufferOut:)

Returns an audio buffer list that contains the media data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferGetAudioBufferListWithRetainedBlockBuffer(
    _ sbuf: CMSampleBuffer,
    bufferListSizeNeededOut: UnsafeMutablePointer?,
    bufferListOut: UnsafeMutablePointer?,
    bufferListSize: Int,
    blockBufferAllocator blockBufferStructureAllocator: CFAllocator?,
    blockBufferMemoryAllocator blockBufferBlockAllocator: CFAllocator?,
    flags: UInt32,
    blockBufferOut: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`sbuf`  

`CMSampleBuffer` being accessed.

`bufferListSizeNeededOut`  

Receives the size of the AudioBufferList required to accommodate the data. May be `NULL`.

`bufferListOut`  

Allocated by the caller, sized as specified by `bufferListSizeNeededOut`. It’s filled in with pointers into the retained `blockBufferOut`. May be `NULL`.

`bufferListSize`  

Size of the `bufferListOut` allocated by the client. If `bufferListOut` isn’t `NULL` and `bufferListSize` is insufficient, `kFigSampleBufferError_ArrayTooSmall` is returned.

`blockBufferStructureAllocator`  

Allocator to use when creating the `CMBlockBuffer` structure.

`blockBufferBlockAllocator`  

Allocator to use for memory block held by the `CMBlockBuffer`.

`flags`  

Flags controlling operation.

`blockBufferOut`  

The retained `CMBlockBuffer`.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

Creates an `AudioBufferList` containing the data from the `CMSampleBuffer`, and a `CMBlockBuffer` which references (and manages the lifetime of) the data in that `AudioBufferList`. The data may or may not be copied, depending on the contiguity and 16-byte alignment of the sample buffer’s data.

The buffers placed in the `AudioBufferList` are guaranteed to be contiguous.

The buffers in the `AudioBufferList` will be 16-byte-aligned if `kCMSampleBufferFlag_AudioBufferList_Assure16ByteAlignment` is passed in.

## See Also

### Modifying Sample Buffers

func CMSampleBufferGetDataBuffer(CMSampleBuffer) -> CMBlockBuffer?

Returns a block buffer that contains the media data.

func CMSampleBufferSetDataBuffer(CMSampleBuffer, newValue: CMBlockBuffer) -> OSStatus

Sets a block buffer of media data on a sample buffer.

func CMSampleBufferGetImageBuffer(CMSampleBuffer) -> CVImageBuffer?

Returns an image buffer that contains the media data.

func CMSampleBufferSetDataBufferFromAudioBufferList(CMSampleBuffer, blockBufferAllocator: CFAllocator?, blockBufferMemoryAllocator: CFAllocator?, flags: UInt32, bufferList: UnsafePointer&lt;AudioBufferList>) -> OSStatus

Creates a block buffer that contains a copy of the data from an audio buffer list.

func CMSampleBufferCopyPCMDataIntoAudioBufferList(CMSampleBuffer, at: Int32, frameCount: Int32, into: UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Copies PCM audio data from a sample buffer into an audio buffer list.

func CMSampleBufferGetAudioStreamPacketDescriptions(CMSampleBuffer, allocatedSize: Int, packetDescriptionsOut: UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, packetDescriptionsSizeNeededOut: UnsafeMutablePointer&lt;Int>?) -> OSStatus

Creates an array of audio stream packet descriptions.

func CMSampleBufferGetAudioStreamPacketDescriptionsPtr(CMSampleBuffer, packetDescriptionsPointerOut: UnsafeMutablePointer&lt;UnsafePointer&lt;AudioStreamPacketDescription>?>?, sizeOut: UnsafeMutablePointer&lt;Int>?) -> OSStatus

Returns a pointer to a constant array of audio stream packet descriptions.

