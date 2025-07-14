

- AppKit
- NSAnimationDelegate
-  animationDidStop(\_:) 

Instance Method

# animationDidStop(\_:)

Sent to the delegate when the specified animation is stopped before it completes its run.

macOS

``` source
nonisolated
optional func animationDidStop(_ animation: NSAnimation)
```

## Parameters 

`animation`  

The `NSAnimation` instance that was stopped.

## Discussion

An `NSAnimation` object stops running when it receives a stop() message.

## See Also

### Controlling and Monitoring an Animation

func animationDidEnd(NSAnimation)

Sent to the delegate when the specified animation completes its run.

func animationShouldStart(NSAnimation) -> Bool

Sent to the delegate just after an animation is started.

func animation(NSAnimation, valueForProgress: NSAnimation.Progress) -> Float

Requests a custom curve value for the current progress value.

