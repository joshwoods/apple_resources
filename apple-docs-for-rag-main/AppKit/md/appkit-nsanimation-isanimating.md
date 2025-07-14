

- AppKit
- NSAnimation
-  isAnimating 

Instance Property

# isAnimating

A Boolean value indicating whether the animation is in progress.

macOS

``` source
var isAnimating: Bool { get }
```

## Discussion

The value of this property is true when the animation is in progress or false when it is stopped.

## See Also

### Controlling and Monitoring an Animation

func start()

Starts the animation represented by the receiver.

func stop()

Stops the animation represented by the receiver.

var currentProgress: NSAnimation.Progress

The current progress of the animation.

var currentValue: Float

The current value of the animation effect, based on the current progress

