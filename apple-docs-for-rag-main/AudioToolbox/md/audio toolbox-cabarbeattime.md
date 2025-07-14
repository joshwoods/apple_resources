

- Audio Toolbox
-  CABarBeatTime 

Structure

# CABarBeatTime

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct CABarBeatTime
```

## Topics

### Initializers

init()

init(bar: Int32, beat: UInt16, subbeat: UInt16, subbeatDivisor: UInt16, reserved: UInt16)

### Instance Properties

var bar: Int32

var beat: UInt16

var reserved: UInt16

var subbeat: UInt16

var subbeatDivisor: UInt16

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Converting Time Values

func CAClockBarBeatTimeToBeats(CAClockRef, UnsafePointer&lt;CABarBeatTime>, UnsafeMutablePointer&lt;CAClockBeats>) -> OSStatus

func CAClockBeatsToBarBeatTime(CAClockRef, CAClockBeats, UInt16, UnsafeMutablePointer&lt;CABarBeatTime>) -> OSStatus

func CAClockSMPTETimeToSeconds(CAClockRef, UnsafePointer&lt;SMPTETime>, UnsafeMutablePointer&lt;CAClockSeconds>) -> OSStatus

func CAClockSecondsToSMPTETime(CAClockRef, CAClockSeconds, UInt16, UnsafeMutablePointer&lt;SMPTETime>) -> OSStatus

func CAClockTranslateTime(CAClockRef, UnsafePointer&lt;CAClockTime>, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

enum CAClockTimebase

typealias CAClockSeconds

typealias CAClockBeats

typealias CAClockSMPTEFormat

struct CAMeterTrackEntry

