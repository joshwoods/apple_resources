

- AVFoundation
- AVOutputSettingsAssistant
-  sourceAudioFormat 

Instance Property

# sourceAudioFormat

The format of the source audio data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var sourceAudioFormat: CMAudioFormatDescription? { get set }
```

## Discussion

The default value is `nil`, which means the assistant doesn’t know the audio format. Setting a value for this property helps the assistant generate more complete audio settings. After setting a value, requery the audioSettings property to get the latest values.

## See Also

### Configuring Output Settings

var outputFileType: AVFileType

A uniform type identifier (UTI) that indicates the type of file to write.

var audioSettings: [String : Any]?

An audio settings dictionary.

var videoSettings: [String : Any]?

A video settings dictionary.

var sourceVideoFormat: CMVideoFormatDescription?

The format of the source video data.

var sourceVideoMinFrameDuration: CMTime

A time value that describes the minimum frame duration of the video data.

var sourceVideoAverageFrameDuration: CMTime

A time value that describes the average frame duration of the video data.

