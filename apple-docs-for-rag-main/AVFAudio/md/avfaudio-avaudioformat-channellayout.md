

- AVFAudio
- AVAudioFormat
-  channelLayout 

Instance Property

# channelLayout

The underlying audio channel layout.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var channelLayout: AVAudioChannelLayout? { get }
```

## Discussion

Only formats with more than two channels require channel layouts.

## See Also

### Getting Audio Format Values

var sampleRate: Double

The audio format sampling rate, in hertz.

var channelCount: AVAudioChannelCount

The number of channels of audio data.

var formatDescription: CMAudioFormatDescription

The audio format description to use with Core Media APIs.

