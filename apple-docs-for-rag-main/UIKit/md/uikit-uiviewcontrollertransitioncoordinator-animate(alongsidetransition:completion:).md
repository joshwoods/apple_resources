

- UIKit
- UIViewControllerTransitionCoordinator
-  animate(alongsideTransition:completion:) 

Instance Method

# animate(alongsideTransition:completion:)

Runs the specified animations at the same time as the view controller transition animations.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func animate(
    alongsideTransition animation: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?,
    completion: ((any UIViewControllerTransitionCoordinatorContext) -> Void)? = nil
) -> Bool
```

**Required**

## Parameters 

`animation`  

A block containing the animations you want to perform. These animations run in the same context as the transition animations and therefore have the same default attributes. You may specify `nil` for this parameter.

The block has no return value and takes the following parameter:

context  
The contextual information for performing the animations. Use this object to get the animation-related information, including the container view in which to run your animations. For more information, see UIViewControllerTransitionCoordinatorContext.

The animation you specify must take place in a view descended from the container view.

`completion`  

The block of code to execute after the transition finishes. You may specify `nil` for this parameter. The block has no return value and takes the following parameter:

context  
The contextual information for performing the animations. Use this object to get the animation-related information, including the container view in which to run your animations. For more information, see UIViewControllerTransitionCoordinatorContext.

## Return Value

true if the animations were successfully queued to run or false if they were not.

## Discussion

Use this method to perform animations that aren’t handled by the animator objects themselves. All of the animations you specify must occur inside the animation context’s container view (or one of its descendants). Use the containerView property of the context object to get the container view. To perform animations in a view that doesn’t descend from the container view, use the animateAlongsideTransition(in:animation:completion:) method instead.

The animations in the `animation` parameter are normally performed concurrently with the view controller transition animations. That behavior applies when the animator object’s animateTransition(using:) method is implemented using UIView-based animations. If the animator object uses Core Animation to animate the layer contents directly, your animations are run shortly after the animateTransition: method returns.

This method returns false when the block in the `animation` parameter can’t be queued to run. The completion block can still run even when this method returns false.

## See Also

### Responding to view controller transition progress

func animateAlongsideTransition(in: UIView?, animation: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?, completion: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?) -> Bool

Runs the specified animations in a view that’s outside of the designated container view.

**Required**

func notifyWhenInteractionChanges((any UIViewControllerTransitionCoordinatorContext) -> Void)

Registers a block to be executed when a transition changes from interactive to non-interactive.

**Required**

func notifyWhenInteractionEnds((any UIViewControllerTransitionCoordinatorContext) -> Void)

Registers a block to be executed when a transition changes from interactive to non-interactive.

**Required**

Deprecated

