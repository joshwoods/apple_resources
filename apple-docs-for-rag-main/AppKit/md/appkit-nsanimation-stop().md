

- AppKit
- NSAnimation
-  stop() 

Instance Method

# stop()

Stops the animation represented by the receiver.

macOS

``` source
func stop()
```

## Discussion

The current progress of the receiver is not reset. When this method is sent to instances of NSViewAnimation (a subclass of `NSAnimation`) the receiver moves to the end frame location.

## See Also

### Related Documentation

func stop(when: NSAnimation, reachesProgress: NSAnimation.Progress)

Stops running the animation represented by the receiver when another animation reaches a specific progress mark.

### Controlling and Monitoring an Animation

func start()

Starts the animation represented by the receiver.

var isAnimating: Bool

A Boolean value indicating whether the animation is in progress.

var currentProgress: NSAnimation.Progress

The current progress of the animation.

var currentValue: Float

The current value of the animation effect, based on the current progress

