

- AVFAudio
- AVAudioSession
-  AVAudioSession.InterruptionType 

Enumeration

# AVAudioSession.InterruptionType

Constants that describe the type of an audio interruption.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
enum InterruptionType
```

## Mentioned in 

Handling audio interruptions

## Topics

### Interruption Types

case began

A type that indicates that the operating system began interrupting the audio session.

case ended

A type that indicates that the operating system ended interrupting the audio session.

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

struct InterruptionOptions

Constants that indicate the state of an audio session after an interruption.

enum InterruptionReason

Constants that define the reasons for an audio session interruption.

