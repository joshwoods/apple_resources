

- UIKit
- UIViewImplicitlyAnimating
-  addCompletion(\_:) 

Instance Method

# addCompletion(\_:)

Adds the specified completion block to the animator.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
optional func addCompletion(_ completion: @escaping (UIViewAnimatingPosition) -> Void)
```

``` source
@MainActor
optional func addCompletion() async -> UIViewAnimatingPosition
```

## Parameters 

`completion`  

A block to execute when the animations finish. This block has no return value and takes the following parameter:

finalPosition  
The position where the animations stopped. Use this value to specify whether the animations stopped at their starting point, their end point, or their current position.

## Discussion

Use this method to add the completion blocks to your custom animator object. Completion blocks should execute after the animations finish successfully. If the stopAnimation(_:) method is called, do not execute any completion blocks if the `withoutFinishing` parameter for that method contains the value true. If the parameter is false and the client subsequent calls the finishAnimation(at:) method, execute the completion blocks in your implementation of that method. Your implementation must be able to handle multiple calls to this method.

## See Also

### Modifying animations

func addAnimations(() -> Void)

Adds the specified animation block to the animator.

func addAnimations(() -> Void, delayFactor: CGFloat)

Adds the specified animation block to the animator with a delay.

func continueAnimation(withTimingParameters: (any UITimingCurveProvider)?, durationFactor: CGFloat)

Adjusts the final timing and duration of a paused animation.

