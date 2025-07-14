

- UIKit
- UIViewController
-  endAppearanceTransition() 

Instance Method

# endAppearanceTransition()

Tells a child controller its appearance has changed.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func endAppearanceTransition()
```

## Discussion

If you are implementing a custom container controller, use this method to tell the child that the view transition is complete.

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

class let hierarchyInconsistencyException: NSExceptionName

Raised if the view controller hierarchy is inconsistent with the view hierarchy.

