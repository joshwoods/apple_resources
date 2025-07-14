

- UIKit
- UIViewController
-  children 

Instance Property

# children

An array of view controllers that are children of the current view controller.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var children: [UIViewController] { get }
```

## Discussion

This property does not include any presented view controllers. This property is only intended to be read by an implementation of a custom container view controller.

## See Also

### Managing child view controllers in a custom container

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

class let hierarchyInconsistencyException: NSExceptionName

Raised if the view controller hierarchy is inconsistent with the view hierarchy.

