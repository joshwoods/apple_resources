

- UIKit
- UIViewControllerAnimatedTransitioning
-  interruptibleAnimator(using:) 

Instance Method

# interruptibleAnimator(using:)

Returns the interruptible animator to use during the transition.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
optional func interruptibleAnimator(using transitionContext: any UIViewControllerContextTransitioning) -> any UIViewImplicitlyAnimating
```

## Parameters 

`transitionContext`  

The context object containing information to use during the transition.

## Return Value

An animator object that supports the modification of its running animations.

## Discussion

Implement this method when you want to perform your transitions using an interruptible animator object, such as a UIViewPropertyAnimator object. You must return the same animator object for the duration of the transition.

