

- Core Audio Types
-  MPEG4ObjectID Deprecated

Enumeration

# MPEG4ObjectID

Constants that define the type of MPEG-4 audio data.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
enum MPEG4ObjectID
```

Deprecated

Deprecated in Mac OS X 10.5.

## Topics

### Constants

case AAC_LC

A constant that specifies lossless coding, which provides compression with no loss of quality.

case AAC_LTP

A constant that specifies long-term prediction, which reduces redundancy in a coded signal.

case aac_Main

A constant that specifies advanced audio coding, which is the basic MPEG-4 technology.

case AAC_SBR

A constant that specifies spectral band replication, which reconstructs high-frequency content from lower frequencies and side information.

case AAC_SSR

A constant that specifies scalable sampling rate, which provides different sampling frequencies for different targets.

case aac_Scalable

A constant that specifies scalable lossless coding.

case CELP

A constant that specifies code-excited linear prediction, which is a narrow-band/wide-band speech codec.

case HVXC

A constant that specifies harmonic vector excitation coding, which is a very-low bit-rate parametric speech codec.

case twinVQ

A constant that specifies transform-domain weighted interleaved vector quantization.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Streams

struct AudioStreamBasicDescription

A format specification for an audio stream.

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

