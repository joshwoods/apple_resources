

- AppKit
- NSAnimation
-  frameRate 

Instance Property

# frameRate

The number of frame updates per second to generate for the animation.

macOS

``` source
var frameRate: Float { get set }
```

## Discussion

The value of this property must be greater than or equal to `0`. Specifying a value of `0.0` causes the animation to run as fast as possible. Setting the property to a negative value raises an exception.

The frame rate is not guaranteed due to differences among systems for the time needed to process a frame. You can change the frame rate while an animation is running and the new value is used at the next frame. The default frame rate is set to a reasonable value (which is subject to future change).

## See Also

### Configuring an Animation

var animationBlockingMode: NSAnimation.BlockingMode

The blocking mode of the animation.

var runLoopModesForAnimating: [RunLoop.Mode]?

An array of strings representing the run loop modes in which the animation can run.

var animationCurve: NSAnimation.Curve

The timing curve for the animation.

var duration: TimeInterval

The duration of the animation, in seconds.

