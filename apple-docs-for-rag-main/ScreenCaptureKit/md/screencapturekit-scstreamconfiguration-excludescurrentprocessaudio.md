

- ScreenCaptureKit
- SCStreamConfiguration
-  excludesCurrentProcessAudio 

Instance Property

# excludesCurrentProcessAudio

A Boolean value that indicates whether to exclude audio from your app during capture.

Mac Catalyst 16.1+macOS 13.0+

``` source
var excludesCurrentProcessAudio: Bool { get set }
```

## Discussion

The default value is false. If you include your app process in the stream output, you can set this value to true to exclude its audio.

## See Also

### Configuring audio

var capturesAudio: Bool

A Boolean value that indicates whether to capture audio.

var sampleRate: Int

The sample rate for audio capture.

var channelCount: Int

The number of audio channels to capture.

