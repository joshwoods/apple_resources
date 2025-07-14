

- AppKit
- NSAnimation
- NSAnimation.BlockingMode
-  NSAnimation.BlockingMode.nonblockingThreaded 

Case

# NSAnimation.BlockingMode.nonblockingThreaded

Requests the animation to run in a separate thread that is spawned by the `NSAnimation` object.

macOS

``` source
case nonblockingThreaded
```

## Discussion

The secondary thread has its own run loop.

## See Also

### Constants

case blocking

Requests the animation to run in the main thread in a custom run-loop mode that blocks user input.

case nonblocking

Requests the animation to run in a standard or specified run-loop mode that allows user input.

