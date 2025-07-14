

- Audio Toolbox
-  CAClockBarBeatTimeToBeats(\_:\_:\_:) 

Function

# CAClockBarBeatTimeToBeats(\_:\_:\_:)

macOS 10.4+

``` source
func CAClockBarBeatTimeToBeats(
    _ inCAClock: CAClockRef,
    _ inBarBeatTime: UnsafePointer,
    _ outBeats: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Converting Time Values

func CAClockBeatsToBarBeatTime(CAClockRef, CAClockBeats, UInt16, UnsafeMutablePointer&lt;CABarBeatTime>) -> OSStatus

func CAClockSMPTETimeToSeconds(CAClockRef, UnsafePointer&lt;SMPTETime>, UnsafeMutablePointer&lt;CAClockSeconds>) -> OSStatus

func CAClockSecondsToSMPTETime(CAClockRef, CAClockSeconds, UInt16, UnsafeMutablePointer&lt;SMPTETime>) -> OSStatus

func CAClockTranslateTime(CAClockRef, UnsafePointer&lt;CAClockTime>, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

enum CAClockTimebase

typealias CAClockSeconds

typealias CAClockBeats

typealias CAClockSMPTEFormat

struct CABarBeatTime

struct CAMeterTrackEntry

