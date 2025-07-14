

- Audio Toolbox
-  CAClockGetPlayRate(\_:\_:) 

Function

# CAClockGetPlayRate(\_:\_:)

macOS 10.4+

``` source
func CAClockGetPlayRate(
    _ inCAClock: CAClockRef,
    _ outPlayRate: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Accessing Tempo Information

func CAClockGetCurrentTempo(CAClockRef, UnsafeMutablePointer&lt;CAClockTempo>, UnsafeMutablePointer&lt;CAClockTime>?) -> OSStatus

func CAClockSetCurrentTempo(CAClockRef, CAClockTempo, UnsafePointer&lt;CAClockTime>?) -> OSStatus

func CAClockSetPlayRate(CAClockRef, Float64) -> OSStatus

typealias CAClockTempo

struct CATempoMapEntry

