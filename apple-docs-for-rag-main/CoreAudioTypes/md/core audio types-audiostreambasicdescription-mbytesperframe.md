

- Core Audio Types
- AudioStreamBasicDescription
-  mBytesPerFrame 

Instance Property

# mBytesPerFrame

The number of bytes from the start of one frame to the start of the next frame in an audio buffer.

iOS 2.0+iPadOS 2.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var mBytesPerFrame: UInt32
```

## Discussion

For an audio buffer containing *interleaved* data for *n* channels, with each sample of type `AudioSampleType`, calculate the value for this field as follows:

```
mBytesPerFrame = n * sizeof (AudioSampleType);
```

For an audio buffer containing *noninterleaved* (monophonic) data, also using `AudioSampleType` samples, calculate the value for this field as follows:

```
mBytesPerFrame = sizeof (AudioSampleType);
```

Set this field to `0` for compressed formats.

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

var mChannelsPerFrame: UInt32

The number of channels in each frame of audio data.

var mBytesPerPacket: UInt32

The number of bytes in a packet of audio data.

var mFramesPerPacket: UInt32

The number of frames in a packet of audio data.

var mReserved: UInt32

The amount to pad the structure to force an even 8-byte alignment.

