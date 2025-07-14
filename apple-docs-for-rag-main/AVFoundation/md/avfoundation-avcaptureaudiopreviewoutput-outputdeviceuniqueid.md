

- AVFoundation
- AVCaptureAudioPreviewOutput
-  outputDeviceUniqueID 

Instance Property

# outputDeviceUniqueID

The unique identifier of the Core Audio output device to use for audio preview.

macOS 10.7+

``` source
var outputDeviceUniqueID: String? { get set }
```

## Discussion

Set the value to the unique identifier of the audio output device, or `nil` to use default system output.

## See Also

### Configuring the Output

var volume: Float

The output volume of the audio preview.

