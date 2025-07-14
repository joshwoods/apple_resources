

- AVFAudio
- AVAudioFormat
-  init(cmAudioFormatDescription:) 

Initializer

# init(cmAudioFormatDescription:)

Creates an audio format instance from a Core Media audio format description.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(cmAudioFormatDescription formatDescription: CMAudioFormatDescription)
```

## Parameters 

`formatDescription`  

The Core Media audio format description.

## Return Value

A new `AVAudioFormat` instance, or `nil` if `formatDescription` isn’t valid.

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

init?(streamDescription: UnsafePointer&lt;AudioStreamBasicDescription>, channelLayout: AVAudioChannelLayout?)

Creates an audio format instance from a stream description and channel layout.

