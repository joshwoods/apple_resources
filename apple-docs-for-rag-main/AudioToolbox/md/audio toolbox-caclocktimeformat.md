

- Audio Toolbox
-  CAClockTimeFormat 

Enumeration

# CAClockTimeFormat

macOS

``` source
enum CAClockTimeFormat
```

## Topics

### Constants

case absoluteSeconds

case beats

case hostTime

case smpteSeconds

case smpteTime

case samples

case seconds

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

### Accessing the Current Time

func CAClockGetCurrentTime(CAClockRef, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

func CAClockSetCurrentTime(CAClockRef, UnsafePointer&lt;CAClockTime>) -> OSStatus

func CAClockGetStartTime(CAClockRef, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

struct CAClockTime

typealias CAClockSamples

