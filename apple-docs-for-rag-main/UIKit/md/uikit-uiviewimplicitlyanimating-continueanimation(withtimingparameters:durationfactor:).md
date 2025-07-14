

- UIKit
- UIViewImplicitlyAnimating
-  continueAnimation(withTimingParameters:durationFactor:) 

Instance Method

# continueAnimation(withTimingParameters:durationFactor:)

Adjusts the final timing and duration of a paused animation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func continueAnimation(
    withTimingParameters parameters: (any UITimingCurveProvider)?,
    durationFactor: CGFloat
)
```

## Parameters 

`parameters`  

The new timing information to apply to the animation. Your custom animator determines how to transition from any current animations to the new animations specified by this parameter.

`durationFactor`  

A multiplying factor to apply to the animation’s original duration. Multiply this value by your animation’s original duration value to obtain the new duration for the animations.

## Discussion

Use this method to change the timing and duration parameters for the current animations temporarily. You define the conditions for which it’s safe to call this method, but typically it’s an error to call this method on an animator that’s inactive, running, or not interruptible. You should retain the original timing and duration values and restore them when your animator transitions back to the inactive state.

## See Also

### Related Documentation

func pauseAnimation()

Pauses a running animation at its current position.

**Required**

### Modifying animations

func addAnimations(() -> Void)

Adds the specified animation block to the animator.

func addAnimations(() -> Void, delayFactor: CGFloat)

Adds the specified animation block to the animator with a delay.

func addCompletion((UIViewAnimatingPosition) -> Void)

Adds the specified completion block to the animator.

