

- AVFoundation
- AVCaptureAudioDataOutput
-  audioSettings 

Instance Property

# audioSettings

The settings used to decode or re-encode audio before it’s output.

macOS 10.7+

``` source
var audioSettings: [String : Any]! { get set }
```

## Discussion

The value of this property is a dictionary containing values for audio settings keys defined in Audio settings.

If the value of this property is `nil`, samples are output in their device native format.

## See Also

### Configuring Audio Capture

func recommendedAudioSettingsForAssetWriter(writingTo: AVFileType) -> [String : Any]?

Specifies the recommended settings for use with an `AVAssetWriterInput`.

