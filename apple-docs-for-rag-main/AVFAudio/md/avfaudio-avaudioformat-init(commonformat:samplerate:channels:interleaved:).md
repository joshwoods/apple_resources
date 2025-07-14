

- AVFAudio
- AVAudioFormat
-  init(commonFormat:sampleRate:channels:interleaved:) 

Initializer

# init(commonFormat:sampleRate:channels:interleaved:)

Creates an audio format instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    commonFormat format: AVAudioCommonFormat,
    sampleRate: Double,
    channels: AVAudioChannelCount,
    interleaved: Bool
)
```

## Parameters 

`format`  

The audio format.

`sampleRate`  

The sampling rate, in hertz.

`channels`  

The channel count.

`interleaved`  

The Boolean value that indicates whether `format` is in an interleaved state.

## Return Value

A new `AVAudioFormat` instance, or `nil` if the initialization fails.

## Discussion

For information about possible `format` values, see AVAudioCommonFormat.

## See Also

### Related Documentation

var sampleRate: Double

The audio format sampling rate, in hertz.

var isInterleaved: Bool

A Boolean value that indicates whether the samples mix into one stream.

var commonFormat: AVAudioCommonFormat

The common format identifier instance.

### Creating a New Audio Format Representation

init(standardFormatWithSampleRate: Double, channelLayout: AVAudioChannelLayout)

Creates an audio format instance as a deinterleaved float with the specified sample rate and channel layout.

init?(standardFormatWithSampleRate: Double, channels: AVAudioChannelCount)

Creates an audio format instance with the specified sample rate and channel count.

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

