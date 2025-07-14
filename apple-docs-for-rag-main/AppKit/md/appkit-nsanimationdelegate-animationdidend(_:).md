

- AppKit
- NSAnimationDelegate
-  animationDidEnd(\_:) 

Instance Method

# animationDidEnd(\_:)

Sent to the delegate when the specified animation completes its run.

macOS

``` source
nonisolated
optional func animationDidEnd(_ animation: NSAnimation)
```

## Parameters 

`animation`  

The `NSAnimation` instance that completed its run.

## Discussion

When an `NSAnimation` object reaches the end of its planned duration, it has a progress value of 1.0.

## See Also

### Related Documentation

var currentProgress: NSAnimation.Progress

The current progress of the animation.

Cocoa Drawing Guide

Animation Programming Guide for Cocoa

### Controlling and Monitoring an Animation

func animationDidStop(NSAnimation)

Sent to the delegate when the specified animation is stopped before it completes its run.

func animationShouldStart(NSAnimation) -> Bool

Sent to the delegate just after an animation is started.

func animation(NSAnimation, valueForProgress: NSAnimation.Progress) -> Float

Requests a custom curve value for the current progress value.

