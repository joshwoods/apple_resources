

- UIKit
- UIViewController
-  shouldAutomaticallyForwardAppearanceMethods 

Instance Property

# shouldAutomaticallyForwardAppearanceMethods

Returns a Boolean value indicating whether appearance methods are forwarded to child view controllers.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var shouldAutomaticallyForwardAppearanceMethods: Bool { get }
```

## Return Value

true if appearance methods are forwarded or false if they are not.

## Discussion

This method is called to determine whether to automatically forward appearance-related containment callbacks to child view controllers.

The default implementation returns true. Subclasses of the UIViewController class that implement containment logic may override this method to control how these methods are forwarded. If you override this method and return false, you are responsible for telling the child when its views are going to appear or disappear. You do this by calling the child view controller’s beginAppearanceTransition(_:animated:) and endAppearanceTransition() methods.

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

func beginAppearanceTransition(Bool, animated: Bool)

Tells a child controller its appearance is about to change.

func endAppearanceTransition()

Tells a child controller its appearance has changed.

class let hierarchyInconsistencyException: NSExceptionName

Raised if the view controller hierarchy is inconsistent with the view hierarchy.

