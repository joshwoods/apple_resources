

- Audio Toolbox
-  kAUVoiceIOProperty_MutedSpeechActivityEventListener 

Global Variable

# kAUVoiceIOProperty_MutedSpeechActivityEventListener

A property to register a listener that the system calls when it detects speech while the user has the microphone muted.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAUVoiceIOProperty_MutedSpeechActivityEventListener: AudioUnitPropertyID { get }
```

## Discussion

To use this API, your app must implement mute using the kAUVoiceIOProperty_MuteOutput property.

## See Also

### Observing muted speech

typealias AUVoiceIOMutedSpeechActivityEventListener

A block that the system calls to indicate speech activity while the user has the microphone muted.

enum AUVoiceIOSpeechActivityEvent

Constants that indicate the state of muted speech.

