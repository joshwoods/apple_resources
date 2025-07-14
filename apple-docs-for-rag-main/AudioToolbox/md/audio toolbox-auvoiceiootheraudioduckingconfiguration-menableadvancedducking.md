

- Audio Toolbox
- AUVoiceIOOtherAudioDuckingConfiguration
-  mEnableAdvancedDucking 

Instance Property

# mEnableAdvancedDucking

A Boolean value that specifies whether to enable advanced ducking.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var mEnableAdvancedDucking: DarwinBoolean
```

## Discussion

Advanced ducking ducks other non-voice audio based on the presence of voice activity from local and remote chat participants.

The default value is false.

## See Also

### Inspecting a configuration

var mDuckingLevel: AUVoiceIOOtherAudioDuckingLevel

The ducking level of other non-voice audio.

