

- AVFAudio
- AVAudioInputNode
-  isVoiceProcessingBypassed 

Instance Property

# isVoiceProcessingBypassed

A Boolean that indicates whether the node bypasses all microphone uplink processing of the voice-processing unit.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var isVoiceProcessingBypassed: Bool { get set }
```

## See Also

### Getting and Setting Voice Processing Properties

var isVoiceProcessingInputMuted: Bool

A Boolean that indicates whether the input of the voice processing unit is in a muted state.

var isVoiceProcessingAGCEnabled: Bool

A Boolean that indicates whether automatic gain control on the processed microphone uplink signal is active.

var voiceProcessingOtherAudioDuckingConfiguration: AVAudioVoiceProcessingOtherAudioDuckingConfiguration

The ducking configuration of nonvoice audio.

struct AVAudioVoiceProcessingOtherAudioDuckingConfiguration

The configuration of ducking non-voice audio.

