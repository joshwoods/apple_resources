

- AVFAudio
-  AVAudioCompressedBuffer 

Class

# AVAudioCompressedBuffer

An object that represents an audio buffer that you use for compressed audio formats.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioCompressedBuffer
```

## Topics

### Creating an Audio Buffer

init(format: AVAudioFormat, packetCapacity: AVAudioPacketCount)

Creates a buffer that contains constant bytes per packet of audio data in a compressed state.

init(format: AVAudioFormat, packetCapacity: AVAudioPacketCount, maximumPacketSize: Int)

Creates a buffer that contains audio data in a compressed state.

### Getting Audio Buffer Properties

var byteCapacity: UInt32

The number of packets the buffer contains.

var byteLength: UInt32

The number of valid bytes in the buffer.

var data: UnsafeMutableRawPointer

The audio buffer’s data bytes.

var maximumPacketSize: Int

The maximum size of a packet, in bytes.

var packetCapacity: AVAudioPacketCount

The total number of packets that the buffer can contain.

var packetCount: AVAudioPacketCount

The number of packets currently in the buffer.

typealias AVAudioPacketCount

The number of packets of audio data.

var packetDescriptions: UnsafeMutablePointer&lt;AudioStreamPacketDescription>?

The buffer’s array of packet descriptions.

## Relationships

### Inherits From

- AVAudioBuffer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Specialized Audio Buffers

class AVAudioPCMBuffer

An object that represents an audio buffer you use with PCM audio formats.

