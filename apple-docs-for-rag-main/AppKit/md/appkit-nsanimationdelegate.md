

- AppKit
-  NSAnimationDelegate 

Protocol

# NSAnimationDelegate

A set of optional methods implemented by delegates of NSAnimation objects.

macOS

``` source
protocol NSAnimationDelegate : NSObjectProtocol
```

## Topics

### Controlling and Monitoring an Animation

func animationDidEnd(NSAnimation)

Sent to the delegate when the specified animation completes its run.

func animationDidStop(NSAnimation)

Sent to the delegate when the specified animation is stopped before it completes its run.

func animationShouldStart(NSAnimation) -> Bool

Sent to the delegate just after an animation is started.

func animation(NSAnimation, valueForProgress: NSAnimation.Progress) -> Float

Requests a custom curve value for the current progress value.

### Managing Progress Marks

func animation(NSAnimation, didReachProgressMark: NSAnimation.Progress)

Sent to the delegate when an animation reaches a specific progress mark.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSTitlebarAccessoryViewController

## See Also

### Custom Animations

class NSAnimation

An object that manages the timing and progress of animations in the user interface.

