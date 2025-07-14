

- AppKit
- NSAnimation
-  runLoopModesForAnimating 

Instance Property

# runLoopModesForAnimating

An array of strings representing the run loop modes in which the animation can run.

macOS

``` source
var runLoopModesForAnimating: [RunLoop.Mode]? { get }
```

## Discussion

The default value of this property is `nil`, which indicates that the animation can be run in the default, modal, or event-tracking modes. The value of this property is ignored if the animation blocking mode is something other than NSAnimation.BlockingMode.nonblocking.

For information about run loop modes and for constants, see RunLoop.

## See Also

### Configuring an Animation

var animationBlockingMode: NSAnimation.BlockingMode

The blocking mode of the animation.

var animationCurve: NSAnimation.Curve

The timing curve for the animation.

var duration: TimeInterval

The duration of the animation, in seconds.

var frameRate: Float

The number of frame updates per second to generate for the animation.

