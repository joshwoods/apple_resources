

- ScreenCaptureKit
- SCStreamConfiguration
-  channelCount 

Instance Property

# channelCount

The number of audio channels to capture.

Mac Catalyst 16.1+macOS 13.0+

``` source
var channelCount: Int { get set }
```

## Discussion

The framework supports channel counts of `1` (mono) or `2` (stereo). If you don’t specify a channel count, or specify an unsupported value, the system defaults to stereo audio capture.

## See Also

### Configuring audio

var capturesAudio: Bool

A Boolean value that indicates whether to capture audio.

var sampleRate: Int

The sample rate for audio capture.

var excludesCurrentProcessAudio: Bool

A Boolean value that indicates whether to exclude audio from your app during capture.

