

- HomeKit
- HMCameraStream
-  updateAudioStreamSetting(\_:completionHandler:) 

Instance Method

# updateAudioStreamSetting(\_:completionHandler:)

Updates an audio stream’s settings.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 14.5+visionOS 1.0+watchOS 3.0+

``` source
func updateAudioStreamSetting(
    _ audioStreamSetting: HMCameraAudioStreamSetting,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updateAudioStreamSetting(_ audioStreamSetting: HMCameraAudioStreamSetting) async throws
```

## Parameters 

`audioStreamSetting`  

The new audio stream configuration.

`completion`  

The block executed after processing the request.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Configuring the audio stream

var audioStreamSetting: HMCameraAudioStreamSetting

The stream’s current audio setting.

func setAudioStreamSetting(HMCameraAudioStreamSetting)Deprecated

enum HMCameraAudioStreamSetting

The options associated with a camera’s audio stream.

