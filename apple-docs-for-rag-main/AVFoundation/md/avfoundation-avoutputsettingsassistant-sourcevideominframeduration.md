

- AVFoundation
- AVOutputSettingsAssistant
-  sourceVideoMinFrameDuration 

Instance Property

# sourceVideoMinFrameDuration

A time value that describes the minimum frame duration of the video data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var sourceVideoMinFrameDuration: CMTime { get set }
```

## Discussion

Setting this property enables the output settings assistant to generate more complete video settings. After setting a value, requery the videoSettings property to get the latest values.

If the source of the video data is an instance of AVAssetReaderOutput, you can discover the minimum frame duration of your source asset using the AVAssetTrack instance’s minFrameDuration property.

The default value is `1/30`, which means the output settings assistant assumes that the source video has a maximum frame rate of 30fps.

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

var sourceVideoFormat: CMVideoFormatDescription?

The format of the source video data.

var sourceVideoAverageFrameDuration: CMTime

A time value that describes the average frame duration of the video data.

