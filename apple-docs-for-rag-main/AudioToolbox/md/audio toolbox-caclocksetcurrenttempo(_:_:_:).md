

- Audio Toolbox
-  CAClockSetCurrentTempo(\_:\_:\_:) 

Function

# CAClockSetCurrentTempo(\_:\_:\_:)

macOS 10.4+

``` source
func CAClockSetCurrentTempo(
    _ inCAClock: CAClockRef,
    _ inTempo: CAClockTempo,
    _ inTimestamp: UnsafePointer?
) -> OSStatus
```

## See Also

### Accessing Tempo Information

func CAClockGetCurrentTempo(CAClockRef, UnsafeMutablePointer&lt;CAClockTempo>, UnsafeMutablePointer&lt;CAClockTime>?) -> OSStatus

func CAClockGetPlayRate(CAClockRef, UnsafeMutablePointer&lt;Float64>) -> OSStatus

func CAClockSetPlayRate(CAClockRef, Float64) -> OSStatus

typealias CAClockTempo

struct CATempoMapEntry

