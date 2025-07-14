

- UIKit
- UIViewControllerTransitionCoordinator
-  notifyWhenInteractionEnds(\_:) Deprecated

Instance Method

# notifyWhenInteractionEnds(\_:)

Registers a block to be executed when a transition changes from interactive to non-interactive.

iOS 7.0–10.0DeprecatediPadOS 7.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
func notifyWhenInteractionEnds(_ handler: @escaping (any UIViewControllerTransitionCoordinatorContext) -> Void)
```

**Required**

## Parameters 

`handler`  

The block to execute when the transition changes from interactive to noninteractive. The block has no return value and takes the following parameter:

context  
The contextual information for performing the animations. Use this object to get the animation-related information. For more information, see UIViewControllerTransitionCoordinatorContext.

## Discussion

Your block is executed both when the transition completes normally and when the user cancels the transition. In the case where the user cancels the transition, UIKit executes your `context` block, calls the viewWillDisappear(_:) method on the presented view controller, and finally calls the viewWillAppear(_:) method on the original view controller to signal that it’s once again visible.

Inside your block, you can get the value of the isCancelled method of the transition coordinator context and use that value to determine the appropriate course of action. For example, if the transition was canceled, you might use this block to remove any extra views that were added to the view hierarchy by a previous call to animate(alongsideTransition:completion:) or animateAlongsideTransition(in:animation:completion:).

You can call this method multiple times to register multiple blocks. All of the registered blocks are executed when the transition state changes.

## See Also

### Responding to view controller transition progress

func animate(alongsideTransition: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?, completion: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?) -> Bool

Runs the specified animations at the same time as the view controller transition animations.

**Required**

func animateAlongsideTransition(in: UIView?, animation: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?, completion: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?) -> Bool

Runs the specified animations in a view that’s outside of the designated container view.

**Required**

func notifyWhenInteractionChanges((any UIViewControllerTransitionCoordinatorContext) -> Void)

Registers a block to be executed when a transition changes from interactive to non-interactive.

**Required**

