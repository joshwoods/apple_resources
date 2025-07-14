

- Audio Toolbox
-  CAClockPropertyID 

Enumeration

# CAClockPropertyID

macOS

``` source
enum CAClockPropertyID
```

## Topics

### Constants

case internalTimebase

case midiClockDestinations

case mtcDestinations

case mtcFreewheelTime

case meterTrack

case name

case smpteFormat

case smpteOffset

case sendMIDISPP

case syncMode

case syncSource

case tempoMap

case timebaseSource

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

### Accessing Clock Properties

func CAClockGetProperty(CAClockRef, CAClockPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func CAClockGetPropertyInfo(CAClockRef, CAClockPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

func CAClockSetProperty(CAClockRef, CAClockPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

enum CAClockSyncMode

