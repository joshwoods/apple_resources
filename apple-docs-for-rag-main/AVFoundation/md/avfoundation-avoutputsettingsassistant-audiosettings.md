

- AVFoundation
- AVOutputSettingsAssistant
-  audioSettings 

Instance Property

# audioSettings

An audio settings dictionary.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var audioSettings: [String : Any]? { get }
```

## Discussion

The value of this property may change as a result of setting a new value for the sourceAudioFormat property. See Audio settings for keys and values.

## See Also

### Configuring Output Settings

var outputFileType: AVFileType

A uniform type identifier (UTI) that indicates the type of file to write.

var sourceAudioFormat: CMAudioFormatDescription?

The format of the source audio data.

var videoSettings: [String : Any]?

A video settings dictionary.

var sourceVideoFormat: CMVideoFormatDescription?

The format of the source video data.

var sourceVideoMinFrameDuration: CMTime

A time value that describes the minimum frame duration of the video data.

var sourceVideoAverageFrameDuration: CMTime

A time value that describes the average frame duration of the video data.

