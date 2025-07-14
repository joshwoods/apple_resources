

- HomeKit
-  HMCameraAudioStreamSetting 

Enumeration

# HMCameraAudioStreamSetting

The options associated with a camera’s audio stream.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
enum HMCameraAudioStreamSetting
```

## Topics

### Configuring the Audio Stream

case muted

The setting that mutes both incoming and outgoing audio.

case incomingAudioAllowed

The setting that permits incoming audio.

case bidirectionalAudioAllowed

The setting that permits both incoming and outgoing audio.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the audio stream

var audioStreamSetting: HMCameraAudioStreamSetting

The stream’s current audio setting.

func updateAudioStreamSetting(HMCameraAudioStreamSetting, completionHandler: ((any Error)?) -> Void)

Updates an audio stream’s settings.

func setAudioStreamSetting(HMCameraAudioStreamSetting)Deprecated

