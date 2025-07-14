

- UIKit
- UIViewController
-  beginAppearanceTransition(\_:animated:) 

Instance Method

# beginAppearanceTransition(\_:animated:)

Tells a child controller its appearance is about to change.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func beginAppearanceTransition(
    _ isAppearing: Bool,
    animated: Bool
)
```

## Parameters 

`isAppearing`  

true if the child view controller’s view is about to be added to the view hierarchy, false if it is being removed.

`animated`  

If true, the transition is being animated.

## Discussion

If you are implementing a custom container controller, use this method to tell the child that its views are about to appear or disappear. Do not invoke viewWillAppear(_:), viewWillDisappear(_:), viewDidAppear(_:), or viewDidDisappear(_:) directly.

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

func endAppearanceTransition()

Tells a child controller its appearance has changed.

class let hierarchyInconsistencyException: NSExceptionName

Raised if the view controller hierarchy is inconsistent with the view hierarchy.

