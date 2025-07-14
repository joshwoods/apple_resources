

- UIKit
- UIViewPropertyAnimator
-  addCompletion(\_:) 

Instance Method

# addCompletion(\_:)

Adds the specified completion block to the animator.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
func addCompletion(_ completion: @escaping (UIViewAnimatingPosition) -> Void)
```

``` source
@MainActor
func addCompletion() async -> UIViewAnimatingPosition
```

## Parameters 

`completion`  

A block to execute when the animations finish. This block has no return value and takes the following parameter:

finalPosition  
The ending position of the animations. Use this value to determine whether the animations stopped at the beginning, end, or somewhere in the middle.

## Discussion

Completion blocks are executed after the animations finish normally. If you call the stopAnimation(_:) method, the completion blocks are not called if you specify true for the method’s parameter. If you specify false for the parameter, the animator executes the completion blocks normally after you call the its finishAnimation(at:) method.

You may add completion blocks to an animator at any time, including while it is stopped.

## See Also

### Modifying animations

func addAnimations(() -> Void)

Adds the specified animation block to the animator.

func addAnimations(() -> Void, delayFactor: CGFloat)

Adds the specified animation block with a delay.

func continueAnimation(withTimingParameters: (any UITimingCurveProvider)?, durationFactor: CGFloat)

Adjusts the timing and duration of a paused animation.

