

- AVFAudio
- AVAudioFormat
-  init(streamDescription:channelLayout:) 

Initializer

# init(streamDescription:channelLayout:)

Creates an audio format instance from a stream description and channel layout.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    streamDescription asbd: UnsafePointer,
    channelLayout layout: AVAudioChannelLayout?
)
```

## Parameters 

`asbd`  

The audio stream description.

`layout`  

The channel layout.

## Return Value

A new `AVAudioFormat` instance, or `nil` if the initialization fails.

## Discussion

When `layout` is `nil`, and `asbd` specifies one or two channels, this method assumes mono or stereo layout, respectively.

If the AudioStreamBasicDescription specifies more than two channels and `layout` is `nil`, this method fails and returns `nil`.

## See Also

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

init(cmAudioFormatDescription: CMAudioFormatDescription)

Creates an audio format instance from a Core Media audio format description.

