

- UIKit
- UIViewController
-  hierarchyInconsistencyException 

Type Property

# hierarchyInconsistencyException

Raised if the view controller hierarchy is inconsistent with the view hierarchy.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
class let hierarchyInconsistencyException: NSExceptionName
```

## Discussion

When a view controller’s view is added to the view hierarchy, the system walks up the view hierarchy to find the first parent view that has a view controller. That view controller must be the parent of the view controller whose view is being added. Otherwise, this exception is raised. This consistency check is also performed when a view controller is added as a child by calling the addChild(_:) method.

It is also allowed for a view controller that has no parent to add its view to the view hierarchy. This is generally not recommended, but is useful in some special cases.

## See Also

### Managing child view controllers in a custom container

var children: [UIViewController]

An array of view controllers that are children of the current view controller.

func addChild(UIViewController)

Adds the specified view controller as a child of the current view controller.

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

