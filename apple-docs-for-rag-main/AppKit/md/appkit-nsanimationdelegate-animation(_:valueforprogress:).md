

- AppKit
- NSAnimationDelegate
-  animation(\_:valueForProgress:) 

Instance Method

# animation(\_:valueForProgress:)

Requests a custom curve value for the current progress value.

macOS

``` source
nonisolated
optional func animation(
    _ animation: NSAnimation,
    valueForProgress progress: NSAnimation.Progress
) -> Float
```

## Parameters 

`animation`  

An `NSAnimation` object that is running.

`progress`  

A `float` value (typed as `NSAnimationProgress`) that indicates a progress mark of `animation`. This value is always between 0.0 and 1.0.

## Return Value

A `float` value representing a custom curve.

## Discussion

The delegate can compute and return a custom curve value for the given progress value. If the delegate does not implement this method, `NSAnimation` computes the current curve value.

The animation:valueForProgress: message is sent to the delegate when an `NSAnimation` object receives a currentValue message. The value the delegate returns is used as the value of currentValue; if there is no delegate, or it doesn’t implement animation:valueForProgress:, `NSAnimation` computes and returns the current value. `NSAnimation` does not invoke currentValueitself, but subclasses might.

See the description of currentValue for more information.

## See Also

### Related Documentation

var currentValue: Float

The current value of the animation effect, based on the current progress

### Controlling and Monitoring an Animation

func animationDidEnd(NSAnimation)

Sent to the delegate when the specified animation completes its run.

func animationDidStop(NSAnimation)

Sent to the delegate when the specified animation is stopped before it completes its run.

func animationShouldStart(NSAnimation) -> Bool

Sent to the delegate just after an animation is started.

