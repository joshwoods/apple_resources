

- ScreenCaptureKit
- SCStreamConfiguration
-  capturesAudio 

Instance Property

# capturesAudio

A Boolean value that indicates whether to capture audio.

Mac Catalyst 16.1+macOS 13.0+

``` source
var capturesAudio: Bool { get set }
```

## Discussion

A stream doesn’t capture audio by default. Set this value to true if you require audio capture.

## See Also

### Configuring audio

var sampleRate: Int

The sample rate for audio capture.

var channelCount: Int

The number of audio channels to capture.

var excludesCurrentProcessAudio: Bool

A Boolean value that indicates whether to exclude audio from your app during capture.

