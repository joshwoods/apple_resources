

- AppKit
- NSAnimation
-  start() 

Instance Method

# start()

Starts the animation represented by the receiver.

macOS

``` source
func start()
```

## Discussion

A strong reference to the animation is maintained until the end of the animation or until its stop() method is called. If the blocking mode is NSAnimation.BlockingMode.blocking, this method returns after the animation has completed or the delegate sends it stop(). If the receiver has a progress of `1.0`, it starts again at `0.0`.

## See Also

### Related Documentation

func start(when: NSAnimation, reachesProgress: NSAnimation.Progress)

Starts running the animation represented by the receiver when another animation reaches a specific progress mark.

### Controlling and Monitoring an Animation

func stop()

Stops the animation represented by the receiver.

var isAnimating: Bool

A Boolean value indicating whether the animation is in progress.

var currentProgress: NSAnimation.Progress

The current progress of the animation.

var currentValue: Float

The current value of the animation effect, based on the current progress

