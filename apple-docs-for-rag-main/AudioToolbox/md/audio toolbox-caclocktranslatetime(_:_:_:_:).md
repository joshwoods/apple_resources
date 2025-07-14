

- Audio Toolbox
-  CAClockTranslateTime(\_:\_:\_:\_:) 

Function

# CAClockTranslateTime(\_:\_:\_:\_:)

macOS 10.4+

``` source
func CAClockTranslateTime(
    _ inCAClock: CAClockRef,
    _ inTime: UnsafePointer,
    _ inOutputTimeFormat: CAClockTimeFormat,
    _ outTime: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Converting Time Values

func CAClockBarBeatTimeToBeats(CAClockRef, UnsafePointer&lt;CABarBeatTime>, UnsafeMutablePointer&lt;CAClockBeats>) -> OSStatus

func CAClockBeatsToBarBeatTime(CAClockRef, CAClockBeats, UInt16, UnsafeMutablePointer&lt;CABarBeatTime>) -> OSStatus

func CAClockSMPTETimeToSeconds(CAClockRef, UnsafePointer&lt;SMPTETime>, UnsafeMutablePointer&lt;CAClockSeconds>) -> OSStatus

func CAClockSecondsToSMPTETime(CAClockRef, CAClockSeconds, UInt16, UnsafeMutablePointer&lt;SMPTETime>) -> OSStatus

enum CAClockTimebase

typealias CAClockSeconds

typealias CAClockBeats

typealias CAClockSMPTEFormat

struct CABarBeatTime

struct CAMeterTrackEntry

