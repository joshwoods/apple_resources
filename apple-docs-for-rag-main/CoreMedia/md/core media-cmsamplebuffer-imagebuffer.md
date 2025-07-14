

- Core Media
- CMSampleBuffer
-  imageBuffer 

Instance Property

# imageBuffer

An image buffer that contains the media data.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var imageBuffer: CVImageBuffer? { get }
```

## Discussion

The value is nil if the sample buffer doesn’t contain a CVImageBuffer, if the sample contains a CMBlockBuffer APIs, or if there’s an error.

## See Also

### Modifying Sample Buffers

var dataBuffer: CMBlockBuffer?

A block buffer that contains the media data.

func setDataBuffer(CMBlockBuffer) throws

Associates a block buffer of media data with a sample buffer.

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

func singleSampleBuffers() throws -> CMSampleBuffer.SingleSampleBuffers

Returns all samples in a sample buffer.

struct SingleSampleBuffers

A structure that holds all samples in a sample buffer.

