

- Core Media
- CMSampleBuffer
-  copyPCMData(fromRange:into:) 

Instance Method

# copyPCMData(fromRange:into:)

Copies PCM audio data from a sample buffer into a prepopulated audio buffer list.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func copyPCMData(
    fromRange range: Range,
    into bufferList: UnsafeMutablePointer
) throws
```

## Parameters 

`range`  

The range of the data buffer to copy from.

`bufferList`  

The audio buffer list to populate.

## Discussion

The audio buffer list must contain the same number of channels, and must be appropriately sized for its data buffers to hold the specified number of frames. This API is specific to audio format sample buffers, and throws an invalidMediaTypeForOperation if called with a nonaudio sample buffer. Likewise, this method throws an error if the sample buffer doesn’t contain PCM audio data or if its data buffer isn’t ready.

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

func audioStreamPacketDescriptions() throws -> [AudioStreamPacketDescription]

Creates an array of audio stream packet descriptions for the variable bytes per packet or variable frames per packet audio data in a sample buffer.

func withUnsafeAudioStreamPacketDescriptions&lt;R>((UnsafeBufferPointer&lt;AudioStreamPacketDescription>) throws -> R) throws -> R

Calls a closure with an audio stream packet description.

func singleSampleBuffers() throws -> CMSampleBuffer.SingleSampleBuffers

Returns all samples in a sample buffer.

struct SingleSampleBuffers

A structure that holds all samples in a sample buffer.

