

- Audio Toolbox
-  CAClockSMPTETimeToSeconds(\_:\_:\_:) 

Function

# CAClockSMPTETimeToSeconds(\_:\_:\_:)

macOS 10.4+

``` source
func CAClockSMPTETimeToSeconds(
    _ inCAClock: CAClockRef,
    _ inSMPTETime: UnsafePointer,
    _ outSeconds: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Converting Time Values

func CAClockBarBeatTimeToBeats(CAClockRef, UnsafePointer&lt;CABarBeatTime>, UnsafeMutablePointer&lt;CAClockBeats>) -> OSStatus

func CAClockBeatsToBarBeatTime(CAClockRef, CAClockBeats, UInt16, UnsafeMutablePointer&lt;CABarBeatTime>) -> OSStatus

func CAClockSecondsToSMPTETime(CAClockRef, CAClockSeconds, UInt16, UnsafeMutablePointer&lt;SMPTETime>) -> OSStatus

func CAClockTranslateTime(CAClockRef, UnsafePointer&lt;CAClockTime>, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

enum CAClockTimebase

typealias CAClockSeconds

typealias CAClockBeats

typealias CAClockSMPTEFormat

struct CABarBeatTime

struct CAMeterTrackEntry

