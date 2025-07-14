

- AVFAudio
- AVAudioSession
-  AVAudioSession.InterruptionOptions 

Structure

# AVAudioSession.InterruptionOptions

Constants that indicate the state of an audio session after an interruption.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
struct InterruptionOptions
```

## Mentioned in 

Handling audio interruptions

## Topics

### Creating an Interruption Option

init(rawValue: UInt)

Creates a new instance with the raw value you specify.

### Getting Standard Interruption Options

static var shouldResume: AVAudioSession.InterruptionOptions

An option that indicates the interruption by another audio session has ended and the app can resume its audio session.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### User Info Values

enum InterruptionType

Constants that describe the type of an audio interruption.

enum InterruptionReason

Constants that define the reasons for an audio session interruption.

