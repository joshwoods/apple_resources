

- AVFAudio
-  AVAudioPacketCount 

Type Alias

# AVAudioPacketCount

The number of packets of audio data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias AVAudioPacketCount = UInt32
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

var packetCount: AVAudioPacketCount

The number of packets currently in the buffer.

var packetDescriptions: UnsafeMutablePointer&lt;AudioStreamPacketDescription>?

The buffer’s array of packet descriptions.

