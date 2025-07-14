

- Audio Toolbox
-  CAClockSetCurrentTime(\_:\_:) 

Function

# CAClockSetCurrentTime(\_:\_:)

macOS 10.4+

``` source
func CAClockSetCurrentTime(
    _ inCAClock: CAClockRef,
    _ inTime: UnsafePointer
) -> OSStatus
```

## See Also

### Accessing the Current Time

func CAClockGetCurrentTime(CAClockRef, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

func CAClockGetStartTime(CAClockRef, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

struct CAClockTime

enum CAClockTimeFormat

typealias CAClockSamples

