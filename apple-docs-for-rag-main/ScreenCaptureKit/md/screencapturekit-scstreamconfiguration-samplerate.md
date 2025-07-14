

- ScreenCaptureKit
- SCStreamConfiguration
-  sampleRate 

Instance Property

# sampleRate

The sample rate for audio capture.

Mac Catalyst 16.1+macOS 13.0+

``` source
var sampleRate: Int { get set }
```

## Discussion

The framework supports sample rates of `8000`, `16000`, `24000`, and `48000`. If you don’t specify a sample rate, or specify an unsupported value, the system uses a default sample rate of 48 kHz.

## See Also

### Configuring audio

var capturesAudio: Bool

A Boolean value that indicates whether to capture audio.

var channelCount: Int

The number of audio channels to capture.

var excludesCurrentProcessAudio: Bool

A Boolean value that indicates whether to exclude audio from your app during capture.

