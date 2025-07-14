

- Audio Toolbox
-  CAClockBeatsToBarBeatTime(\_:\_:\_:\_:) 

Function

# CAClockBeatsToBarBeatTime(\_:\_:\_:\_:)

macOS 10.4+

``` source
func CAClockBeatsToBarBeatTime(
    _ inCAClock: CAClockRef,
    _ inBeats: CAClockBeats,
    _ inSubbeatDivisor: UInt16,
    _ outBarBeatTime: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Converting Time Values

func CAClockBarBeatTimeToBeats(CAClockRef, UnsafePointer&lt;CABarBeatTime>, UnsafeMutablePointer&lt;CAClockBeats>) -> OSStatus

func CAClockSMPTETimeToSeconds(CAClockRef, UnsafePointer&lt;SMPTETime>, UnsafeMutablePointer&lt;CAClockSeconds>) -> OSStatus

func CAClockSecondsToSMPTETime(CAClockRef, CAClockSeconds, UInt16, UnsafeMutablePointer&lt;SMPTETime>) -> OSStatus

func CAClockTranslateTime(CAClockRef, UnsafePointer&lt;CAClockTime>, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

enum CAClockTimebase

typealias CAClockSeconds

typealias CAClockBeats

typealias CAClockSMPTEFormat

struct CABarBeatTime

struct CAMeterTrackEntry

