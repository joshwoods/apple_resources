

- AVFAudio
- AVAudioVoiceProcessingOtherAudioDuckingConfiguration
-  enableAdvancedDucking 

Instance Property

# enableAdvancedDucking

Enables advanced ducking which ducks other audio based on the presence of voice activity from local and remote chat participants.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var enableAdvancedDucking: ObjCBool
```

## See Also

### Configuring ducking

var duckingLevel: AVAudioVoiceProcessingOtherAudioDuckingConfiguration.Level

The ducking level of other audio.

enum Level

Constants that define the supported ducking levels.

