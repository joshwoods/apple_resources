

- AVFAudio
- AVAudioSession
-  AVAudioSession.InterruptionReason 

Enumeration

# AVAudioSession.InterruptionReason

Constants that define the reasons for an audio session interruption.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
enum InterruptionReason
```

## Topics

### Interruption Reasons

case `default`

The system interrupts this audio session when it activates another.

case builtInMicMuted

The system interrupts the audio session when the device mutes the built-in microphone.

case routeDisconnected

The system interrupts the audio session due to a disconnection of an audio route.

case appWasSuspended

The system suspends the app and interrupts the audio session.

Deprecated

case sceneWasBackgrounded

The system backgrounds the scene and interrupts the audio session.

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

### User Info Values

enum InterruptionType

Constants that describe the type of an audio interruption.

struct InterruptionOptions

Constants that indicate the state of an audio session after an interruption.

