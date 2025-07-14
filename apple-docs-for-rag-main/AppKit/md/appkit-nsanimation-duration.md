

- AppKit
- NSAnimation
-  duration 

Instance Property

# duration

The duration of the animation, in seconds.

macOS

``` source
var duration: TimeInterval { get set }
```

## Discussion

The value of this property must be greater than or equal to `0`. Setting the duration to a negative value raises an exception.

You can change the duration of an animation while it is running. Setting the duration to a value that is less than the current progress value ends an in-progress animation.

## See Also

### Configuring an Animation

var animationBlockingMode: NSAnimation.BlockingMode

The blocking mode of the animation.

var runLoopModesForAnimating: [RunLoop.Mode]?

An array of strings representing the run loop modes in which the animation can run.

var animationCurve: NSAnimation.Curve

The timing curve for the animation.

var frameRate: Float

The number of frame updates per second to generate for the animation.

