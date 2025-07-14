

- Core Media
- CMSampleBuffer
-  setDataBuffer(fromAudioBufferList:blockBufferMemoryAllocator:flags:) 

Instance Method

# setDataBuffer(fromAudioBufferList:blockBufferMemoryAllocator:flags:)

Creates a block buffer that contains a copy of the data from an audio buffer list, and sets it as the sample buffer’s data.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func setDataBuffer(
    fromAudioBufferList bufferList: UnsafePointer,
    blockBufferMemoryAllocator: CFAllocator? = kCFAllocatorDefault,
    flags: CMSampleBuffer.Flags = []
) throws
```

## Parameters 

`bufferList`  

The audio buffer list from which to copy the data.

`blockBufferMemoryAllocator`  

An allocator to use for the memory block that the block buffer holds.

`flags`  

Optional flags that control the operation.

## Discussion

Pass the audioBufferListAssure16ByteAlignment flag to have the system create 16-byte-aligned buffers.

## See Also

### Modifying Sample Buffers

var dataBuffer: CMBlockBuffer?

A block buffer that contains the media data.

func setDataBuffer(CMBlockBuffer) throws

Associates a block buffer of media data with a sample buffer.

var imageBuffer: CVImageBuffer?

An image buffer that contains the media data.

func withAudioBufferList&lt;R>(blockBufferMemoryAllocator: CFAllocator?, flags: CMSampleBuffer.Flags, body: (UnsafeMutableAudioBufferListPointer, CMBlockBuffer) throws -> R) throws -> R

Calls a closure with an audio buffer list that contains the data from a sample buffer and a block buffer backing the audio buffers.

func copyPCMData(fromRange: Range&lt;Int>, into: UnsafeMutablePointer&lt;AudioBufferList>) throws

Copies PCM audio data from a sample buffer into a prepopulated audio buffer list.

func audioStreamPacketDescriptions() throws -> [AudioStreamPacketDescription]

Creates an array of audio stream packet descriptions for the variable bytes per packet or variable frames per packet audio data in a sample buffer.

func withUnsafeAudioStreamPacketDescriptions&lt;R>((UnsafeBufferPointer&lt;AudioStreamPacketDescription>) throws -> R) throws -> R

Calls a closure with an audio stream packet description.

func singleSampleBuffers() throws -> CMSampleBuffer.SingleSampleBuffers

Returns all samples in a sample buffer.

struct SingleSampleBuffers

A structure that holds all samples in a sample buffer.

