

- Audio Toolbox
-  CAClockSMPTEFormat 

Type Alias

# CAClockSMPTEFormat

macOS

``` source
typealias CAClockSMPTEFormat = SMPTETimeType
```

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

struct CABarBeatTime

struct CAMeterTrackEntry

