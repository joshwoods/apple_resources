

- AVFAudio
- AVAudioCompressedBuffer
-  init(format:packetCapacity:maximumPacketSize:) 

Initializer

# init(format:packetCapacity:maximumPacketSize:)

Creates a buffer that contains audio data in a compressed state.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    format: AVAudioFormat,
    packetCapacity: AVAudioPacketCount,
    maximumPacketSize: Int
)
```

## Parameters 

`format`  

The format of the audio the buffer contains.

`packetCapacity`  

The capacity of the buffer, in packets.

`maximumPacketSize`  

The maximum size in bytes of a packet in a compressed state.

## Return Value

A new AVAudioCompressedBuffer instance.

## Discussion

You can obtain the maximum packet size from the maximumOutputPacketSize property of an AVAudioConverter you configure for encoding this format.

The method raises an exception if the format is PCM.

## See Also

### Creating an Audio Buffer

init(format: AVAudioFormat, packetCapacity: AVAudioPacketCount)

Creates a buffer that contains constant bytes per packet of audio data in a compressed state.

