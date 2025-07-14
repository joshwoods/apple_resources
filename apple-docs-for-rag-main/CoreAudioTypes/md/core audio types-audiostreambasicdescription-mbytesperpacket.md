

- Core Audio Types
- AudioStreamBasicDescription
-  mBytesPerPacket 

Instance Property

# mBytesPerPacket

The number of bytes in a packet of audio data.

iOS 2.0+iPadOS 2.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var mBytesPerPacket: UInt32
```

## Discussion

To indicate variable packet size, set this field to `0`. For a format that uses variable packet size, specify the size of each packet using an AudioStreamPacketDescription structure.

## See Also

### Inspecting a description

var mFormatID: AudioFormatID

An identifier specifying the general audio data format in the stream.

var mFormatFlags: AudioFormatFlags

Format-specific flags to specify details of the format.

var mSampleRate: Float64

The number of frames per second of the data in the stream, when playing the stream at normal speed.

var mBitsPerChannel: UInt32

The number of bits for one audio sample.

var mBytesPerFrame: UInt32

The number of bytes from the start of one frame to the start of the next frame in an audio buffer.

var mChannelsPerFrame: UInt32

The number of channels in each frame of audio data.

var mFramesPerPacket: UInt32

The number of frames in a packet of audio data.

var mReserved: UInt32

The amount to pad the structure to force an even 8-byte alignment.

