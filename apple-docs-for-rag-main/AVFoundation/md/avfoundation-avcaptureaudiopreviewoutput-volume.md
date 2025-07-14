

- AVFoundation
- AVCaptureAudioPreviewOutput
-  volume 

Instance Property

# volume

The output volume of the audio preview.

macOS 10.7+

``` source
var volume: Float { get set }
```

## Discussion

A value of `1.0` indicates maximum volume, and a value of `0.0` mutes the audio preview.

## See Also

### Configuring the Output

var outputDeviceUniqueID: String?

The unique identifier of the Core Audio output device to use for audio preview.

