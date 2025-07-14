

- Audio Toolbox
-  CAClockGetCurrentTime(\_:\_:\_:) 

Function

# CAClockGetCurrentTime(\_:\_:\_:)

macOS 10.4+

``` source
func CAClockGetCurrentTime(
    _ inCAClock: CAClockRef,
    _ inTimeFormat: CAClockTimeFormat,
    _ outTime: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Accessing the Current Time

func CAClockSetCurrentTime(CAClockRef, UnsafePointer&lt;CAClockTime>) -> OSStatus

func CAClockGetStartTime(CAClockRef, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

struct CAClockTime

enum CAClockTimeFormat

typealias CAClockSamples

