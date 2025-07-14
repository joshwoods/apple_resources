

- AppKit
- NSAnimationDelegate
-  animationShouldStart(\_:) 

Instance Method

# animationShouldStart(\_:)

Sent to the delegate just after an animation is started.

macOS

``` source
nonisolated
optional func animationShouldStart(_ animation: NSAnimation) -> Bool
```

## Parameters 

`animation`  

The `NSAnimation` object that was just started.

## Return Value

false to cancel the animation, true to have the animation proceed.

## Discussion

The delegate is sent this message just after `animation` receives a start() message. The delegate can use this method to prepare objects and resources for the effect.

## See Also

### Controlling and Monitoring an Animation

func animationDidEnd(NSAnimation)

Sent to the delegate when the specified animation completes its run.

func animationDidStop(NSAnimation)

Sent to the delegate when the specified animation is stopped before it completes its run.

func animation(NSAnimation, valueForProgress: NSAnimation.Progress) -> Float

Requests a custom curve value for the current progress value.

