

- AppKit
- NSAnimation
- NSAnimation.BlockingMode
-  NSAnimation.BlockingMode.blocking 

Case

# NSAnimation.BlockingMode.blocking

Requests the animation to run in the main thread in a custom run-loop mode that blocks user input.

macOS

``` source
case blocking
```

## Discussion

This is the default.

## See Also

### Constants

case nonblocking

Requests the animation to run in a standard or specified run-loop mode that allows user input.

case nonblockingThreaded

Requests the animation to run in a separate thread that is spawned by the `NSAnimation` object.

