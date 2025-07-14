

- Core Media
- CMSampleBuffer
-  withAudioBufferList(blockBufferMemoryAllocator:flags:body:) 

Instance Method

# withAudioBufferList(blockBufferMemoryAllocator:flags:body:)

Calls a closure with an audio buffer list that contains the data from a sample buffer and a block buffer backing the audio buffers.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func withAudioBufferList(
    blockBufferMemoryAllocator: CFAllocator? = kCFAllocatorDefault,
    flags: CMSampleBuffer.Flags = [],
    body: (UnsafeMutableAudioBufferListPointer, CMBlockBuffer) throws -> R
) throws -> R
```

## Parameters 

`blockBufferMemoryAllocator`  

An allocator to use for the memory block held by a CMBlockBuffer APIs.

`flags`  

Optional flags that control the operation.

`body`  

A closure the system calls that contains a pointer to an AudioBufferList and the block buffer that backs its audio buffers.

## Discussion

The system may not copy the data, depending on its contiguity and 16-byte alignment. It guarantees the buffers it places in the AudioBufferList are contiguous.

The system returns 16-byte-aligned buffers if you pass the audioBufferListAssure16ByteAlignment flag.

## See Also

### Modifying Sample Buffers

var dataBuffer: CMBlockBuffer?

A block buffer that contains the media data.

func setDataBuffer(CMBlockBuffer) throws

Associates a block buffer of media data with a sample buffer.

var imageBuffer: CVImageBuffer?

An image buffer that contains the media data.

func setDataBuffer(fromAudioBufferList: UnsafePointer&lt;AudioBufferList>, blockBufferMemoryAllocator: CFAllocator?, flags: CMSampleBuffer.Flags) throws

Creates a block buffer that contains a copy of the data from an audio buffer list, and sets it as the sample buffer’s data.

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

