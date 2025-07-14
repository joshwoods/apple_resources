

- UIKit
- UIViewPropertyAnimator
-  addAnimations(\_:) 

Instance Method

# addAnimations(\_:)

Adds the specified animation block to the animator.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
func addAnimations(_ animation: @escaping () -> Void)
```

## Parameters 

`animation`  

A block containing the animations you want to add to the animator object. This block has no return value and takes no parameters. This parameter must not be `nil`.

## Discussion

Use this method to add new animation blocks to the animator. The animations in the new block run alongside any previously configured animations. Blocks added while the animator’s state is UIViewAnimatingState.inactive are executed over the time specified by the duration property. Blocks added while the animator’s state is UIViewAnimatingState.active are executed over the remaining portion of the total run time. For example, if the duration is `2.0` and you add an animation block to a running animator whose fractionComplete property is `0.5`, the animations run for `1.0` second. Any blocks you add while the animator is running begin executing immediately.

If the `animation` block modifies a property that’s being modified by a different property animator, then the animators combine their changes in the most appropriate way. For many properties, the changes from each animator are added together to yield a new intermediate value. If a property can’t be modified in this additive manner, the new animations take over as if the beginFromCurrentState option had been specified for a view-based animation.

You can call this method multiple times to add multiple blocks to the animator. It’s a programmer error to call this method when the animator’s state property is set to UIViewAnimatingState.stopped.

## See Also

### Modifying animations

func addAnimations(() -> Void, delayFactor: CGFloat)

Adds the specified animation block with a delay.

func addCompletion((UIViewAnimatingPosition) -> Void)

Adds the specified completion block to the animator.

func continueAnimation(withTimingParameters: (any UITimingCurveProvider)?, durationFactor: CGFloat)

Adjusts the timing and duration of a paused animation.

