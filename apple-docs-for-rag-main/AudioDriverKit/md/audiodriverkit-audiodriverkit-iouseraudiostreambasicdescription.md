

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioStreamBasicDescription 

Structure

# IOUserAudioStreamBasicDescription

A structure that encapsulates all of the information for describing the basic format properties of a stream of audio data.

DriverKit 21.0+

``` source
struct IOUserAudioStreamBasicDescription;
```

## Discussion

This structure contains the information needed to describe any constant bit rate format that has channels that are the same size. For variable bit rate data and for constant bit rate data where the channels have unequal sizes, the type requires more data than this type provides. However, where applicable, the framework fills out the appropriate fields correctly for these kinds of formats using separate properties for the additional data.

In all fields, a value of `0` indicates that the field is either unknown, not applicable, or otherwise is inapproprate for the format. The mFormatFlags field is an exception to this, where `0` is still a valid value for most formats.

In audio data a frame is one sample across all channels. In non-interleaved audio, the per frame fields identify one channel. In interleaved audio, the per-frame fields identify the set of `n` channels. In uncompressed audio, a packet is one frame, (`mFramesPerPacket == 1`). In compressed audio, a packet is an indivisible chunk of compressed data, for example an AAC packet contains 1024 sample frames.

## Topics

### Accessing the Sample Rate

mSampleRate

The number of sample frames per second of the data in the stream.

### Identifying the Format

mFormatID

The audio format identifier indicating the general kind of data in the stream.

IOUserAudioFormatID

An enumeration of four character codes used to identify distinct audio data formats.

mFormatFlags

Audio format flags for the stream’s format.

IOUserAudioFormatFlags

Flag values that provide more information about the format used by an audio stream basic description.

### Accessing Packet and Frame Layout

mBytesPerPacket

The byte count in each packet of data.

mFramesPerPacket

The number of sample frames in each packet of data.

mBytesPerFrame

The byte count in each frame of data.

mChannelsPerFrame

The number of channels in each frame of data.

mBitsPerChannel

The number of bits of sample data for each channel in a frame of data.

### Infrequently Used Properties

mReserved

An unused field reserved for future use.

## See Also

### Working with Stream Formats

SetCurrentStreamFormat

Sets the current stream format to a given audio stream basic description.

GetCurrentStreamFormat

Returns the current stream format, as an audio stream basic description.

SetAvailableStreamFormats

Sets the available stream formats to an array of audio stream basic descriptions.

GetAvailableStreamFormats

Returns the available stream formats as an array of audio stream basic descriptions.

GetNumberAvailableStreamFormats

Returns the number of available stream formats.

GetStreamDirection

Gets the direction of the stream: input or output.

IOUserAudioStreamDirection

A type representing the direction of audio flow.

SetStreamIsActive

Sets a Boolean value that indicates whether the stream is active and doing I/O.

GetStreamIsActive

Gets a value that indicates whether the stream is active and doing I/O.

