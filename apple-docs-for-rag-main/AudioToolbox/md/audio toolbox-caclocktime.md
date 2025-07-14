

- Audio Toolbox
-  CAClockTime 

Structure

# CAClockTime

macOS

``` source
struct CAClockTime
```

## Topics

### Initializers

init()

init(format: CAClockTimeFormat, reserved: UInt32, time: CAClockTime.__Unnamed_union_time)

### Instance Properties

var format: CAClockTimeFormat

var reserved: UInt32

var time: CAClockTime.__Unnamed_union_time

## Relationships

### Conforms To

- Sendable

## See Also

### Accessing the Current Time

func CAClockGetCurrentTime(CAClockRef, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

func CAClockSetCurrentTime(CAClockRef, UnsafePointer&lt;CAClockTime>) -> OSStatus

func CAClockGetStartTime(CAClockRef, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

enum CAClockTimeFormat

typealias CAClockSamples

