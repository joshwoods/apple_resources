

- AppKit
- NSAnimation
-  animationBlockingMode 

Instance Property

# animationBlockingMode

The blocking mode of the animation.

macOS

``` source
var animationBlockingMode: NSAnimation.BlockingMode { get set }
```

## Discussion

The value in this property determines whether the animation blocks a given thread. The default value of this property is NSAnimation.BlockingMode.blocking, which means that the animation runs on the main thread in a custom run-loop mode that blocks user events. When changing the value of this property, the new blocking mode takes effect the next time the animation is started and has no effect on an in-progress animation.

If you set the block mode to NSAnimation.BlockingMode.nonblocking, the animation runs in the main thread in one of the standard run-loop modes or in a mode returned from NSAnimation. If you set the mode to NSAnimation.BlockingMode.nonblockingThreaded, a new thread is spawned to run the animation.

## See Also

### Configuring an Animation

var runLoopModesForAnimating: [RunLoop.Mode]?

An array of strings representing the run loop modes in which the animation can run.

var animationCurve: NSAnimation.Curve

The timing curve for the animation.

var duration: TimeInterval

The duration of the animation, in seconds.

var frameRate: Float

The number of frame updates per second to generate for the animation.

