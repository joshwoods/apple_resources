

- UIKit
- UIViewControllerTransitionCoordinator
-  animateAlongsideTransition(in:animation:completion:) 

Instance Method

# animateAlongsideTransition(in:animation:completion:)

Runs the specified animations in a view that’s outside of the designated container view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func animateAlongsideTransition(
    in view: UIView?,
    animation: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?,
    completion: ((any UIViewControllerTransitionCoordinatorContext) -> Void)? = nil
) -> Bool
```

**Required**

## Parameters 

`view`  

The view (or one of its ancestors) in which the specified animations take place. This parameter must not be `nil`.

`animation`  

A block containing the animations you want to perform. These animations run in the same context as the transition animations and therefore have the same default attributes. You may specify `nil` for this parameter.

The block has no return value and takes the following parameter:

context  
The contextual information for performing the animations. Use this object to get the animation-related information. For more information, see UIViewControllerTransitionCoordinatorContext.

`completion`  

The block of code to execute after the transition finishes. You may specify `nil` for this parameter. The block has no return value and takes the following parameter:

context  
The contextual information for performing the animations. Use this object to get the animation-related information. For more information, see UIViewControllerTransitionCoordinatorContext.

## Return Value

true if the specified animation is successfully queued to run; otherwise false.

## Discussion

Use this method to perform animations that aren’t handled by the animator objects themselves. The animations you specify in the `animation` parameter must all take place in a view descended from the view you specify in the `view` parameter.

The animations in the `animation` parameter are normally performed concurrently with the view controller transition animations. That behavior applies when the animator object’s animateTransition(using:) method is implemented using UIView-based animations. If the animator object uses Core Animation to animate the layer contents directly, your animations are run shortly after the animateTransition: method returns.

This method returns false when the block in the `animation` parameter can’t be queued to run. The completion block can still run even when this method returns false.

## See Also

### Responding to view controller transition progress

func animate(alongsideTransition: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?, completion: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?) -> Bool

Runs the specified animations at the same time as the view controller transition animations.

**Required**

func notifyWhenInteractionChanges((any UIViewControllerTransitionCoordinatorContext) -> Void)

Registers a block to be executed when a transition changes from interactive to non-interactive.

**Required**

func notifyWhenInteractionEnds((any UIViewControllerTransitionCoordinatorContext) -> Void)

Registers a block to be executed when a transition changes from interactive to non-interactive.

**Required**

Deprecated

