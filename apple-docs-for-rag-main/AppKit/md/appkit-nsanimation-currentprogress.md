

- AppKit
- NSAnimation
-  currentProgress 

Instance Property

# currentProgress

The current progress of the animation.

macOS

``` source
var currentProgress: NSAnimation.Progress { get set }
```

## Discussion

This property contains the completion percentage of the animation. Valid values are in the range `0.0` to `1.0`, where `0.0` represents the beginning of the animation and `1.0` represents the end of the animation.

Changing the value of this property adjusts the progress of a running animation. Setting this property to a value less than `0.0` sets the value of the property to `0.0`. Similarly, specifying a value greater than `1.0` changes the value of the property to `1.0`. The `NSAnimation` class updates the value of this property during the animation. To perform additional tasks at specific progress points, use the delegate’s animation(_:valueForProgress:) method.

## See Also

### Controlling and Monitoring an Animation

func start()

Starts the animation represented by the receiver.

func stop()

Stops the animation represented by the receiver.

var isAnimating: Bool

A Boolean value indicating whether the animation is in progress.

var currentValue: Float

The current value of the animation effect, based on the current progress

