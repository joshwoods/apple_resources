

- HomeKit
- HMCameraStream
-  audioStreamSetting 

Instance Property

# audioStreamSetting

The stream’s current audio setting.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 14.5+visionOS 1.0+watchOS 3.0+

``` source
var audioStreamSetting: HMCameraAudioStreamSetting { get }
```

## See Also

### Configuring the audio stream

func updateAudioStreamSetting(HMCameraAudioStreamSetting, completionHandler: ((any Error)?) -> Void)

Updates an audio stream’s settings.

func setAudioStreamSetting(HMCameraAudioStreamSetting)Deprecated

enum HMCameraAudioStreamSetting

The options associated with a camera’s audio stream.

