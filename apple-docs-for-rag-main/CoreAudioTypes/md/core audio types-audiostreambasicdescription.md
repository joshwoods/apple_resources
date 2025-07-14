

- Core Audio Types
-  AudioStreamBasicDescription 

Structure

# AudioStreamBasicDescription

A format specification for an audio stream.

iOS 2.0+iPadOS 2.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
struct AudioStreamBasicDescription
```

## Overview

You can configure an audio stream basic description (ASBD) to specify a linear PCM format or a constant bit rate (CBR) format that has channels of equal size. For variable bit rate (VBR) audio, and for CBR audio where the channels have unequal sizes, also use an AudioStreamPacketDescription structure to additionally describe each packet.

A field value of `0` indicates that the value is either unknown or not applicable to the format.

Always initialize the fields of a new audio stream basic description structure to `0`, as the example below shows:

```
```

To determine the duration that one packet represents, use the mSampleRate field with the mFramesPerPacket field, as follows:

```
```

In Core Audio, the following definitions apply:

- An *audio stream* is a continuous series of data that represents a sound, such as a song.

- A *channel* is a discrete track of monophonic audio. A monophonic stream has one channel; a stereo stream has two channels.

- A *sample* is single numerical value for a single audio channel in an audio stream.

- A *frame* is a collection of time-coincident samples. For instance, a linear PCM stereo sound file has two samples per frame, one for the left channel and one for the right channel.

- A *packet* is a collection of one or more contiguous frames. A packet defines the smallest meaningful set of frames for a given audio data format, and is the smallest data unit for which time can be measured. In linear PCM audio, a packet holds a single frame. In compressed formats, it typically holds more frames. In some formats, the number of frames per packet varies.

- The *sample rate* for a stream is the number of frames per second of uncompressed audio, or, for compressed formats, the equivalent in decompressed audio.

## Topics

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

var mBytesPerPacket: UInt32

The number of bytes in a packet of audio data.

var mFramesPerPacket: UInt32

The number of frames in a packet of audio data.

var mReserved: UInt32

The amount to pad the structure to force an even 8-byte alignment.

### Initializers

init()

Creates an empty description.

init(mSampleRate: Float64, mFormatID: AudioFormatID, mFormatFlags: AudioFormatFlags, mBytesPerPacket: UInt32, mFramesPerPacket: UInt32, mBytesPerFrame: UInt32, mChannelsPerFrame: UInt32, mBitsPerChannel: UInt32, mReserved: UInt32)

Creates a description with the specified values.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Streams

struct AudioStreamPacketDescription

A value that describes a packet in a buffer of audio data.

typealias AudioFormatFlags

A type definition for audio format flags.

Audio Format Flags

Commonly used combinations of data format flags for an audio stream description.

typealias AudioFormatID

A type definition for audio format identifiers.

Audio Format Identifiers

Identifiers for supported audio formats.

let kAudioStreamAnyRate: Float64

A value that indicates that an audio stream can use any sample rate.

enum MPEG4ObjectID

Constants that define the type of MPEG-4 audio data.

Deprecated

