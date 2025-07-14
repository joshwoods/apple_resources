

- Audio Toolbox
-  CAClockGetCurrentTempo(\_:\_:\_:) 

Function

# CAClockGetCurrentTempo(\_:\_:\_:)

macOS 10.4+

``` source
func CAClockGetCurrentTempo(
    _ inCAClock: CAClockRef,
    _ outTempo: UnsafeMutablePointer,
    _ outTimestamp: UnsafeMutablePointer?
) -> OSStatus
```

## See Also

### Accessing Tempo Information

func CAClockSetCurrentTempo(CAClockRef, CAClockTempo, UnsafePointer&lt;CAClockTime>?) -> OSStatus

func CAClockGetPlayRate(CAClockRef, UnsafeMutablePointer&lt;Float64>) -> OSStatus

func CAClockSetPlayRate(CAClockRef, Float64) -> OSStatus

typealias CAClockTempo

struct CATempoMapEntry

