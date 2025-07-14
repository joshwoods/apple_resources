

- AVFAudio
- AVAudioInputNode
-  voiceProcessingOtherAudioDuckingConfiguration 

Instance Property

# voiceProcessingOtherAudioDuckingConfiguration

The ducking configuration of nonvoice audio.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var voiceProcessingOtherAudioDuckingConfiguration: AVAudioVoiceProcessingOtherAudioDuckingConfiguration { get set }
```

## Discussion

Use this property to configures the ducking of nonvoice audio, including advanced enablement and ducking level. Typically, when playing other audio during voice chat, applying a higher level of ducking can increase the intelligibility of the voice chat.

If not set, the default behavior is to disable advanced ducking, with a ducking level set to AVAudioVoiceProcessingOtherAudioDuckingConfiguration.Level.default.

## See Also

### Getting and Setting Voice Processing Properties

var isVoiceProcessingInputMuted: Bool

A Boolean that indicates whether the input of the voice processing unit is in a muted state.

var isVoiceProcessingBypassed: Bool

A Boolean that indicates whether the node bypasses all microphone uplink processing of the voice-processing unit.

var isVoiceProcessingAGCEnabled: Bool

A Boolean that indicates whether automatic gain control on the processed microphone uplink signal is active.

struct AVAudioVoiceProcessingOtherAudioDuckingConfiguration

The configuration of ducking non-voice audio.

