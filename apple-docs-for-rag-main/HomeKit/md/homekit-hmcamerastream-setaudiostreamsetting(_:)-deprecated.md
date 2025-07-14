

- HomeKit
- HMCameraStream
-  setAudioStreamSetting(\_:) Deprecated

Instance Method

# setAudioStreamSetting(\_:)

iOS 10.0–10.0DeprecatediPadOS 10.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
func setAudioStreamSetting(_ audioStreamSetting: HMCameraAudioStreamSetting)
```

Deprecated

Use updateAudioStreamSetting(_:completionHandler:) instead.

## Parameters 

`audioStreamSetting`  

The new audio stream configuration.

## See Also

### Configuring the audio stream

var audioStreamSetting: HMCameraAudioStreamSetting

The stream’s current audio setting.

func updateAudioStreamSetting(HMCameraAudioStreamSetting, completionHandler: ((any Error)?) -> Void)

Updates an audio stream’s settings.

enum HMCameraAudioStreamSetting

The options associated with a camera’s audio stream.

