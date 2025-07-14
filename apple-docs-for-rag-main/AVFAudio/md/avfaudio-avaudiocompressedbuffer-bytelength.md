

- AVFAudio
- AVAudioCompressedBuffer
-  byteLength 

Instance Property

# byteLength

The number of valid bytes in the buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var byteLength: UInt32 { get set }
```

## Discussion

You can change this value as part of an operation that modifies the contents.

## See Also

### Getting Audio Buffer Properties

var byteCapacity: UInt32

The number of packets the buffer contains.

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

