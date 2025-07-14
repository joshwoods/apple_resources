

- AVFoundation
- AVPlayerItem
-  step(byCount:) 

Instance Method

# step(byCount:)

Moves the player item’s current time forward or backward by a specified number of steps.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
func step(byCount stepCount: Int)
```

## Parameters 

`stepCount`  

The number of steps by which to move.

A positive number steps forward, a negative number steps backward.

## Discussion

The size of each step depends on the receiver’s enabled `AVPlayerItemTrack` objects (see tracks).

## See Also

### Stepping Through Media

var canStepForward: Bool

A Boolean value that indicates whether the item supports stepping forward.

var canStepBackward: Bool

A Boolean value that indicates whether the item supports stepping backward.

