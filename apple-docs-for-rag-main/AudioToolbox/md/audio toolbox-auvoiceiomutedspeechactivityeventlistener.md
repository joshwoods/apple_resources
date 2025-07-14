

- Audio Toolbox
-  AUVoiceIOMutedSpeechActivityEventListener 

Type Alias

# AUVoiceIOMutedSpeechActivityEventListener

A block that the system calls to indicate speech activity while the user has the microphone muted.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AUVoiceIOMutedSpeechActivityEventListener = (AUVoiceIOSpeechActivityEvent) -> Void
```

## Parameters 

`event`  

An event that indicates whether muted speech started or ended.

## See Also

### Observing muted speech

var kAUVoiceIOProperty_MutedSpeechActivityEventListener: AudioUnitPropertyID

A property to register a listener that the system calls when it detects speech while the user has the microphone muted.

enum AUVoiceIOSpeechActivityEvent

Constants that indicate the state of muted speech.

