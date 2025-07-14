

- Audio Toolbox
-  AUVoiceIOSpeechActivityEvent 

Enumeration

# AUVoiceIOSpeechActivityEvent

Constants that indicate the state of muted speech.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum AUVoiceIOSpeechActivityEvent
```

## Topics

### Determining when muted speech starts and stops

case hasStarted

A state that indicates speech started.

case hasEnded

A state that indicates speech ended.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Observing muted speech

var kAUVoiceIOProperty_MutedSpeechActivityEventListener: AudioUnitPropertyID

A property to register a listener that the system calls when it detects speech while the user has the microphone muted.

typealias AUVoiceIOMutedSpeechActivityEventListener

A block that the system calls to indicate speech activity while the user has the microphone muted.

