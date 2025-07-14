

- Core Media
-  CMSampleBufferGetDataBuffer(\_:) 

Function

# CMSampleBufferGetDataBuffer(\_:)

Returns a block buffer that contains the media data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferGetDataBuffer(_ sbuf: CMSampleBuffer) -> CMBlockBuffer?
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being interrogated.

## Return Value

`CMBlockBuffer` of media data. The result will be `NULL` if the `CMSampleBuffer` does not contain a `CMBlockBuffer`, if the `CMSampleBuffer` contains a `CVImageBuffer`, or if there is some other error.

## Discussion

The caller doesn’t own the returned `dataBuffer`, and must retain it explicitly if the caller needs to maintain a reference to it.

## See Also

### Modifying Sample Buffers

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

func CMSampleBufferGetAudioStreamPacketDescriptionsPtr(CMSampleBuffer, packetDescriptionsPointerOut: UnsafeMutablePointer&lt;UnsafePointer&lt;AudioStreamPacketDescription>?>?, sizeOut: UnsafeMutablePointer&lt;Int>?) -> OSStatus

Returns a pointer to a constant array of audio stream packet descriptions.

