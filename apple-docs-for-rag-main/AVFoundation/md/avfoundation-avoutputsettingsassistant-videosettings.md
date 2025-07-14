

- AVFoundation
- AVOutputSettingsAssistant
-  videoSettings 

Instance Property

# videoSettings

A video settings dictionary.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var videoSettings: [String : Any]? { get }
```

## Discussion

The value of this property may change as a result of setting a new value for the sourceVideoFormat property. See Video settings for the supported keys and values.

## See Also

### Configuring Output Settings

var outputFileType: AVFileType

A uniform type identifier (UTI) that indicates the type of file to write.

var audioSettings: [String : Any]?

An audio settings dictionary.

var sourceAudioFormat: CMAudioFormatDescription?

The format of the source audio data.

var sourceVideoFormat: CMVideoFormatDescription?

The format of the source video data.

var sourceVideoMinFrameDuration: CMTime

A time value that describes the minimum frame duration of the video data.

var sourceVideoAverageFrameDuration: CMTime

A time value that describes the average frame duration of the video data.

