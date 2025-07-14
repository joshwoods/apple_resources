

- UIKit
- UIViewControllerTransitionCoordinator
-  notifyWhenInteractionChanges(\_:) 

Instance Method

# notifyWhenInteractionChanges(\_:)

Registers a block to be executed when a transition changes from interactive to non-interactive.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
func notifyWhenInteractionChanges(_ handler: @escaping (any UIViewControllerTransitionCoordinatorContext) -> Void)
```

**Required**

## Parameters 

`handler`  

The block to execute when the transition changes from interactive to noninteractive. The block has no return value and takes the following parameter:

## Discussion

Your handler block is executed any time the transition changes from interactive to noninteractive, including when the transition ends or is canceled. When the user cancels a transition, UIKit executes your context block, calls the viewWillDisappear(_:) method on the presented view controller, and finally calls the viewWillAppear(_:) method on the original view controller to signal that it’s once again visible.

Use the isInteractive property of the context object to determine the current interactivity of the transition. You can also use the value of the isCancelled property to determine an appropriate course of action. For example, if the transition was canceled, you might remove any extra views that were added to the view hierarchy by a previous call to animate(alongsideTransition:completion:) or animateAlongsideTransition(in:animation:completion:).

You can call this method multiple times to register multiple blocks. All of the registered blocks are executed when the transition state changes.

## See Also

### Responding to view controller transition progress

func animate(alongsideTransition: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?, completion: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?) -> Bool

Runs the specified animations at the same time as the view controller transition animations.

**Required**

func animateAlongsideTransition(in: UIView?, animation: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?, completion: ((any UIViewControllerTransitionCoordinatorContext) -> Void)?) -> Bool

Runs the specified animations in a view that’s outside of the designated container view.

**Required**

func notifyWhenInteractionEnds((any UIViewControllerTransitionCoordinatorContext) -> Void)

Registers a block to be executed when a transition changes from interactive to non-interactive.

**Required**

Deprecated

