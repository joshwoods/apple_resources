

- Audio Toolbox
-  CAClockSamples 

Type Alias

# CAClockSamples

macOS

``` source
typealias CAClockSamples = Float64
```

## See Also

### Accessing the Current Time

func CAClockGetCurrentTime(CAClockRef, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

func CAClockSetCurrentTime(CAClockRef, UnsafePointer&lt;CAClockTime>) -> OSStatus

func CAClockGetStartTime(CAClockRef, CAClockTimeFormat, UnsafeMutablePointer&lt;CAClockTime>) -> OSStatus

struct CAClockTime

enum CAClockTimeFormat

