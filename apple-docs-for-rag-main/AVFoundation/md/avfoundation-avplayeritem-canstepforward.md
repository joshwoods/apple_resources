

- AVFoundation
- AVPlayerItem
-  canStepForward 

Instance Property

# canStepForward

A Boolean value that indicates whether the item supports stepping forward.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
nonisolated
var canStepForward: Bool { get }
```

## Discussion

Once the item becomes ready to play, the value of this property does not change. This behavior applies even when boundary conditions, such as when the item’s current time is equal to its end time, have been reached.

## See Also

### Stepping Through Media

var canStepBackward: Bool

A Boolean value that indicates whether the item supports stepping backward.

func step(byCount: Int)

Moves the player item’s current time forward or backward by a specified number of steps.

