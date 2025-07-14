

- Core Media
- CMSampleBuffer
-  singleSampleBuffers() 

Instance Method

# singleSampleBuffers()

Returns all samples in a sample buffer.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func singleSampleBuffers() throws -> CMSampleBuffer.SingleSampleBuffers
```

## Return Value

All samples from the buffer.

## Discussion

The system creates temporary sample buffers for individual samples that refer to the sample data and containing its timing, size, and attachments.

If there are no sample sizes in the provided sample buffer, the system throws a kCMSampleBufferError_CannotSubdivide error. This happens, for example, if the samples in the buffer are noncontiguous, such as noninterleaved audio.

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

func setDataBuffer(fromAudioBufferList: UnsafePointer&lt;AudioBufferList>, blockBufferMemoryAllocator: CFAllocator?, flags: CMSampleBuffer.Flags) throws

Creates a block buffer that contains a copy of the data from an audio buffer list, and sets it as the sample buffer’s data.

func copyPCMData(fromRange: Range&lt;Int>, into: UnsafeMutablePointer&lt;AudioBufferList>) throws

Copies PCM audio data from a sample buffer into a prepopulated audio buffer list.

func audioStreamPacketDescriptions() throws -> [AudioStreamPacketDescription]

Creates an array of audio stream packet descriptions for the variable bytes per packet or variable frames per packet audio data in a sample buffer.

func withUnsafeAudioStreamPacketDescriptions&lt;R>((UnsafeBufferPointer&lt;AudioStreamPacketDescription>) throws -> R) throws -> R

Calls a closure with an audio stream packet description.

struct SingleSampleBuffers

A structure that holds all samples in a sample buffer.

