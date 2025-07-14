

- Audio Toolbox
-  CAClockSecondsToSMPTETime(\_:\_:\_:\_:) 

Function

# CAClockSecondsToSMPTETime(\_:\_:\_:\_:)

macOS 10.4+

``` source
func CAClockSecondsToSMPTETime(
    _ inCAClock: CAClockRef,
    _ inSeconds: CAClockSeconds,
    _ inSubframeDivisor: UInt16,
    _ outSMPTETime: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Converting Time Values

func CAClockBarBeatTimeToBeats(CAClockRef, UnsafePointer&lt;CABarBeatTime>, UnsafeMutablePointer&lt;CAClockBeats>) -> OSStatus

func CAClockBeatsToBarBeatTime(CAClockRef, CAClockBeats, UInt16, UnsafeMutablePointer&lt;CABarBeatTime>) -> OSStatus

func CAClockSMPTETimeToSeconds(CAClockRef, UnsafePointer&lt;SMPTETime>, UnsafeMutablePointer&lt;CAClockSeconds>) -> OSStatus

func CAClockTranslateTime(CAClockRef, UnsafePointer&lt;CAClockTime>, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

enum CAClockTimebase

typealias CAClockSeconds

typealias CAClockBeats

typealias CAClockSMPTEFormat

struct CABarBeatTime

struct CAMeterTrackEntry

