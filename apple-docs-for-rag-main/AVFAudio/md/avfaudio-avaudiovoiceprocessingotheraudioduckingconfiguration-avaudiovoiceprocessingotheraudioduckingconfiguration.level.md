

- AVFAudio
- AVAudioVoiceProcessingOtherAudioDuckingConfiguration
-  AVAudioVoiceProcessingOtherAudioDuckingConfiguration.Level 

Enumeration

# AVAudioVoiceProcessingOtherAudioDuckingConfiguration.Level

Constants that define the supported ducking levels.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
enum Level
```

## Topics

### Ducking levels

case `default`

The default ducking level for typical voice chat.

case max

Applies maximum ducking to other audio.

case mid

Applies medium ducking to other audio.

case min

Applies minimum ducking to other audio.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring ducking

var enableAdvancedDucking: ObjCBool

Enables advanced ducking which ducks other audio based on the presence of voice activity from local and remote chat participants.

var duckingLevel: AVAudioVoiceProcessingOtherAudioDuckingConfiguration.Level

The ducking level of other audio.

