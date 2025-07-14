

- Audio Toolbox
-  CATempoMapEntry 

Structure

# CATempoMapEntry

macOS

``` source
struct CATempoMapEntry
```

## Topics

### Initializers

init()

init(beats: CAClockBeats, tempoBPM: CAClockTempo)

### Instance Properties

var beats: CAClockBeats

var tempoBPM: CAClockTempo

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Accessing Tempo Information

func CAClockGetCurrentTempo(CAClockRef, UnsafeMutablePointer&lt;CAClockTempo>, UnsafeMutablePointer&lt;CAClockTime>?) -> OSStatus

func CAClockSetCurrentTempo(CAClockRef, CAClockTempo, UnsafePointer&lt;CAClockTime>?) -> OSStatus

func CAClockGetPlayRate(CAClockRef, UnsafeMutablePointer&lt;Float64>) -> OSStatus

func CAClockSetPlayRate(CAClockRef, Float64) -> OSStatus

typealias CAClockTempo

