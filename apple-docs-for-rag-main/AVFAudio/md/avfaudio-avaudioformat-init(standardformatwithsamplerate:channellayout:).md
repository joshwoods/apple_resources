

- AVFAudio
- AVAudioFormat
-  init(standardFormatWithSampleRate:channelLayout:) 

Initializer

# init(standardFormatWithSampleRate:channelLayout:)

Creates an audio format instance as a deinterleaved float with the specified sample rate and channel layout.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    standardFormatWithSampleRate sampleRate: Double,
    channelLayout layout: AVAudioChannelLayout
)
```

## Parameters 

`sampleRate`  

The sampling rate, in hertz.

`layout`  

The channel layout, which must not be `nil`.

## Return Value

A new `AVAudioFormat` instance.

## Discussion

The returned `AVAudioFormat` instance uses the AVAudioCommonFormat.pcmFormatFloat32 format.

## See Also

### Related Documentation

var sampleRate: Double

The audio format sampling rate, in hertz.

var channelLayout: AVAudioChannelLayout?

The underlying audio channel layout.

### Creating a New Audio Format Representation

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

