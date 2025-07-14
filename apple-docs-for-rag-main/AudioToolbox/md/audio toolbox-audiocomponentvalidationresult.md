

- Audio Toolbox
-  AudioComponentValidationResult 

Enumeration

# AudioComponentValidationResult

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum AudioComponentValidationResult
```

## Topics

### Constants

case failed

case passed

case timedOut

case unauthorizedError_Init

case unauthorizedError_Open

case unknown

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

### Validating an Audio Component

func AudioComponentValidate(AudioComponent, CFDictionary?, UnsafeMutablePointer&lt;AudioComponentValidationResult>) -> OSStatus

var kAudioComponentValidationParameter_LoadOutOfProcess: String

