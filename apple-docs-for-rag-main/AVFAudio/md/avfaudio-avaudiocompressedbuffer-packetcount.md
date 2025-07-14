

- AVFAudio
- AVAudioCompressedBuffer
-  packetCount 

Instance Property

# packetCount

The number of packets currently in the buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var packetCount: AVAudioPacketCount { get set }
```

## See Also

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

typealias AVAudioPacketCount

The number of packets of audio data.

var packetDescriptions: UnsafeMutablePointer&lt;AudioStreamPacketDescription>?

The buffer’s array of packet descriptions.

