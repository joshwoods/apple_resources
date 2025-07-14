

- UIKit
- UIViewController
-  addChild(\_:) 

Instance Method

# addChild(\_:)

Adds the specified view controller as a child of the current view controller.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addChild(_ childController: UIViewController)
```

## Parameters 

`childController`  

The view controller to be added as a child.

## Mentioned in 

Creating a custom container view controller

## Discussion

This method creates a parent-child relationship between the current view controller and the object in the `childController` parameter. This relationship is necessary when embedding the child view controller’s view into the current view controller’s content. If the new child view controller is already the child of a container view controller, it is removed from that container before being added.

This method is only intended to be called by an implementation of a custom container view controller. If you override this method, you must call `super` in your implementation.

## See Also

### Managing child view controllers in a custom container

var children: [UIViewController]

An array of view controllers that are children of the current view controller.

func removeFromParent()

Removes the view controller from its parent.

func transition(from: UIViewController, to: UIViewController, duration: TimeInterval, options: UIView.AnimationOptions, animations: (() -> Void)?, completion: ((Bool) -> Void)?)

Transitions between two of the view controller’s child view controllers.

var shouldAutomaticallyForwardAppearanceMethods: Bool

Returns a Boolean value indicating whether appearance methods are forwarded to child view controllers.

func beginAppearanceTransition(Bool, animated: Bool)

Tells a child controller its appearance is about to change.

func endAppearanceTransition()

Tells a child controller its appearance has changed.

class let hierarchyInconsistencyException: NSExceptionName

Raised if the view controller hierarchy is inconsistent with the view hierarchy.

