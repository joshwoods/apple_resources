

- AVFAudio
-  AVAudioVoiceProcessingOtherAudioDuckingConfiguration 

Structure

# AVAudioVoiceProcessingOtherAudioDuckingConfiguration

The configuration of ducking non-voice audio.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct AVAudioVoiceProcessingOtherAudioDuckingConfiguration
```

## Topics

### Configuring ducking

var enableAdvancedDucking: ObjCBool

Enables advanced ducking which ducks other audio based on the presence of voice activity from local and remote chat participants.

var duckingLevel: AVAudioVoiceProcessingOtherAudioDuckingConfiguration.Level

The ducking level of other audio.

enum Level

Constants that define the supported ducking levels.

### Initializers

init()

init(enableAdvancedDucking: ObjCBool, duckingLevel: AVAudioVoiceProcessingOtherAudioDuckingConfiguration.Level)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Getting and Setting Voice Processing Properties

var isVoiceProcessingInputMuted: Bool

A Boolean that indicates whether the input of the voice processing unit is in a muted state.

var isVoiceProcessingBypassed: Bool

A Boolean that indicates whether the node bypasses all microphone uplink processing of the voice-processing unit.

var isVoiceProcessingAGCEnabled: Bool

A Boolean that indicates whether automatic gain control on the processed microphone uplink signal is active.

var voiceProcessingOtherAudioDuckingConfiguration: AVAudioVoiceProcessingOtherAudioDuckingConfiguration

The ducking configuration of nonvoice audio.

