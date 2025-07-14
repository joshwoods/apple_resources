

- Audio Toolbox
-  CAClockGetStartTime(\_:\_:\_:) 

Function

# CAClockGetStartTime(\_:\_:\_:)

macOS 10.4+

``` source
func CAClockGetStartTime(
    _ inCAClock: CAClockRef,
    _ inTimeFormat: CAClockTimeFormat,
    _ outTime: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Accessing the Current Time

func CAClockGetCurrentTime(CAClockRef, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

func CAClockSetCurrentTime(CAClockRef, UnsafePointer&lt;CAClockTime>) -> OSStatus

struct CAClockTime

enum CAClockTimeFormat

typealias CAClockSamples

