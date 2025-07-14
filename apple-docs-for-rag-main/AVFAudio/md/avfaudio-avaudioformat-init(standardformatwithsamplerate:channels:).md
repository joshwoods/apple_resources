

- AVFAudio
- AVAudioFormat
-  init(standardFormatWithSampleRate:channels:) 

Initializer

# init(standardFormatWithSampleRate:channels:)

Creates an audio format instance with the specified sample rate and channel count.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    standardFormatWithSampleRate sampleRate: Double,
    channels: AVAudioChannelCount
)
```

## Parameters 

`sampleRate`  

The sampling rate, in hertz.

`channels`  

The channel count.

## Return Value

A new `AVAudioFormat` instance, or `nil` if the initialization fails.

## Discussion

The returned `AVAudioFormat` instance uses the AVAudioCommonFormat.pcmFormatFloat32 format.

## See Also

### Related Documentation

var sampleRate: Double

The audio format sampling rate, in hertz.

var channelLayout: AVAudioChannelLayout?

The underlying audio channel layout.

### Creating a New Audio Format Representation

init(standardFormatWithSampleRate: Double, channelLayout: AVAudioChannelLayout)

Creates an audio format instance as a deinterleaved float with the specified sample rate and channel layout.

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

