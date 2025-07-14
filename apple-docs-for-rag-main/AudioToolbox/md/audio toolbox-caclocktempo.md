

- Audio Toolbox
-  CAClockTempo 

Type Alias

# CAClockTempo

macOS

``` source
typealias CAClockTempo = Float64
```

## See Also

### Accessing Tempo Information

func CAClockGetCurrentTempo(CAClockRef, UnsafeMutablePointer&lt;CAClockTempo>, UnsafeMutablePointer&lt;CAClockTime>?) -> OSStatus

func CAClockSetCurrentTempo(CAClockRef, CAClockTempo, UnsafePointer&lt;CAClockTime>?) -> OSStatus

func CAClockGetPlayRate(CAClockRef, UnsafeMutablePointer&lt;Float64>) -> OSStatus

func CAClockSetPlayRate(CAClockRef, Float64) -> OSStatus

struct CATempoMapEntry

