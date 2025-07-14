

- ScreenCaptureKit
- SCStreamOutputType
-  SCStreamOutputType.audio 

Case

# SCStreamOutputType.audio

An output type that represents an audio capture sample buffer.

Mac Catalyst 18.2+macOS 13.0+

``` source
case audio
```

## Discussion

A captured sample buffer wraps an AudioBufferList structure that contains the audio samples. The stream configuration’s sampleRate and channelCount property values determine of the format of the audio.

## See Also

### Output types

case screen

An output type that represents a screen capture sample buffer.

