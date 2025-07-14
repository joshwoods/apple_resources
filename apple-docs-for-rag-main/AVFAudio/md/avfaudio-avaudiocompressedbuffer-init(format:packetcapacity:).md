

- AVFAudio
- AVAudioCompressedBuffer
-  init(format:packetCapacity:) 

Initializer

# init(format:packetCapacity:)

Creates a buffer that contains constant bytes per packet of audio data in a compressed state.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    format: AVAudioFormat,
    packetCapacity: AVAudioPacketCount
)
```

## Parameters 

`format`  

The format of the audio the buffer contains.

`packetCapacity`  

The capacity of the buffer, in packets.

## Return Value

A new AVAudioCompressedBuffer instance.

## Discussion

This fails if the format is PCM or if the format has variable bytes per packet (for example, `format.streamDescription->mBytesPerPacket == 0`).

## See Also

### Creating an Audio Buffer

init(format: AVAudioFormat, packetCapacity: AVAudioPacketCount, maximumPacketSize: Int)

Creates a buffer that contains audio data in a compressed state.

