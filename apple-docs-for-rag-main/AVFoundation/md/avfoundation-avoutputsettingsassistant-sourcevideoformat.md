

- AVFoundation
- AVOutputSettingsAssistant
-  sourceVideoFormat 

Instance Property

# sourceVideoFormat

The format of the source video data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var sourceVideoFormat: CMVideoFormatDescription? { get set }
```

## Discussion

The default value is `nil`, which means the assistant doesn’t know the video format. Setting a value for this property helps the assistant generate more complete video settings. After setting a value, requery the videoSettings property to get the latest values.

## See Also

### Configuring Output Settings

var outputFileType: AVFileType

A uniform type identifier (UTI) that indicates the type of file to write.

var audioSettings: [String : Any]?

An audio settings dictionary.

var sourceAudioFormat: CMAudioFormatDescription?

The format of the source audio data.

var videoSettings: [String : Any]?

A video settings dictionary.

var sourceVideoMinFrameDuration: CMTime

A time value that describes the minimum frame duration of the video data.

var sourceVideoAverageFrameDuration: CMTime

A time value that describes the average frame duration of the video data.

