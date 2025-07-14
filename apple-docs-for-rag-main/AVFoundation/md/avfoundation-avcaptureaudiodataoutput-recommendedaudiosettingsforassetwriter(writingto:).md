

- AVFoundation
- AVCaptureAudioDataOutput
-  recommendedAudioSettingsForAssetWriter(writingTo:) 

Instance Method

# recommendedAudioSettingsForAssetWriter(writingTo:)

Specifies the recommended settings for use with an `AVAssetWriterInput`.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
func recommendedAudioSettingsForAssetWriter(writingTo outputFileType: AVFileType) -> [String : Any]?
```

## Parameters 

`outputFileType`  

Specifies the UTI of the file type to be written. See `File Format UTIs` for the defined UTIs.

## Return Value

A fully populated dictionary of keys and values that are compatible with AVAssetWriter.

## Discussion

The value of this property is an `NSDictionary` containing values for compression settings keys defined in Audio settings. This dictionary is suitable for use as the assetWriterInputWithMediaType:outputSettings: method’s `outputSettings` parameter when creating an AVAssetWriterInputPixelBufferAdaptor; for example,

```
```

The dictionary returned contains all necessary keys and values needed to create an AVAssetWriter instance; see the init(mediaType:outputSettings:) method for a more in depth discussion. For QuickTime movie and ISO files, the recommended audio settings will always produce output comparable to that of AVCaptureMovieFileOutput.

The dictionary of settings is dependent on the current configuration of the receiver’s AVCaptureSession and its inputs. The settings dictionary may change if the session’s configuration changes. As such, you should configure your session first, then query the recommended audio settings.

## See Also

### Configuring Audio Capture

var audioSettings: [String : Any]!

The settings used to decode or re-encode audio before it’s output.

