

- Audio Toolbox
-  CAClockSetPlayRate(\_:\_:) 

Function

# CAClockSetPlayRate(\_:\_:)

macOS 10.4+

``` source
func CAClockSetPlayRate(
    _ inCAClock: CAClockRef,
    _ inPlayRate: Float64
) -> OSStatus
```

## See Also

### Accessing Tempo Information

func CAClockGetCurrentTempo(CAClockRef, UnsafeMutablePointer&lt;CAClockTempo>, UnsafeMutablePointer&lt;CAClockTime>?) -> OSStatus

func CAClockSetCurrentTempo(CAClockRef, CAClockTempo, UnsafePointer&lt;CAClockTime>?) -> OSStatus

func CAClockGetPlayRate(CAClockRef, UnsafeMutablePointer&lt;Float64>) -> OSStatus

typealias CAClockTempo

struct CATempoMapEntry

