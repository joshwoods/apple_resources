

- AVFAudio
-  AVAudioFormat 

Class

# AVAudioFormat

An object that describes the representation of an audio format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioFormat
```

## Overview

The AVAudioFormat class wraps Core Audio’s AudioStreamBasicDescription, and includes convenience initializers and accessors for common formats, including Core Audio’s standard deinterleaved 32-bit floating point format.

Instances of this class are immutable.

## Topics

### Creating a New Audio Format Representation

init(standardFormatWithSampleRate: Double, channelLayout: AVAudioChannelLayout)

Creates an audio format instance as a deinterleaved float with the specified sample rate and channel layout.

init?(standardFormatWithSampleRate: Double, channels: AVAudioChannelCount)

Creates an audio format instance with the specified sample rate and channel count.

init?(commonFormat: AVAudioCommonFormat, sampleRate: Double, channels: AVAudioChannelCount, interleaved: Bool)

Creates an audio format instance.

init(commonFormat: AVAudioCommonFormat, sampleRate: Double, interleaved: Bool, channelLayout: AVAudioChannelLayout)

Creates an audio format instance with the specified audio format, sample rate, interleaved state, and channel layout.

init?(settings: [String : Any])

Creates an audio format instance using the specified settings dictionary.

init?(streamDescription: UnsafePointer&lt;AudioStreamBasicDescription>)

Creates an audio format instance from a stream description.

init?(streamDescription: UnsafePointer&lt;AudioStreamBasicDescription>, channelLayout: AVAudioChannelLayout?)

Creates an audio format instance from a stream description and channel layout.

init(cmAudioFormatDescription: CMAudioFormatDescription)

Creates an audio format instance from a Core Media audio format description.

### Getting the Audio Stream Description

var streamDescription: UnsafePointer&lt;AudioStreamBasicDescription>

The audio format properties of a stream of audio data.

### Comparing Instances

func isEqual(Any) -> Bool

Indicates whether the audio format instance and a specified object are functionally equivalent.

### Getting Audio Format Values

var sampleRate: Double

The audio format sampling rate, in hertz.

var channelCount: AVAudioChannelCount

The number of channels of audio data.

var channelLayout: AVAudioChannelLayout?

The underlying audio channel layout.

var formatDescription: CMAudioFormatDescription

The audio format description to use with Core Media APIs.

### Determining the Audio Format

var isInterleaved: Bool

A Boolean value that indicates whether the samples mix into one stream.

var isStandard: Bool

A Boolean value that indicates whether the format is in a deinterleaved native-endian float state.

var commonFormat: AVAudioCommonFormat

The common format identifier instance.

var settings: [String : Any]

A dictionary that represents the format as a dictionary using audio setting keys.

var magicCookie: Data?

An object that contains metadata that encoders and decoders require.

### Constants

enum AVAudioCommonFormat

The format options that describe common audio formats.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Formats

class AVAudioChannelLayout

An object that describes the roles of a set of audio channels.

let AVChannelLayoutKey: String

Linear PCM Format Settings

The audio settings that apply to linear PCM audio formats.

Format Settings

The audio settings that apply to all audio formats that the audio player and recorder classes support.

