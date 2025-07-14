

- UIKit
- UIViewController
-  showDetailViewController(\_:sender:) 

Instance Method

# showDetailViewController(\_:sender:)

Presents a view controller in a secondary (or detail) context.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func showDetailViewController(
    _ vc: UIViewController,
    sender: Any?
)
```

## Parameters 

`vc`  

The current view controller.

`sender`  

The object being acted upon.

## Mentioned in 

Creating a custom container view controller

Customizing the behavior of segue-based presentations

## Discussion

You use this method to decouple the need to display a view controller from the process of actually presenting that view controller onscreen. Using this method, a view controller does not need to know whether it is embedded inside a navigation controller or split-view controller. It calls the same method for both. In a regular environment, the UISplitViewController class overrides this method and installs `vc` as its detail view controller; in a compact environment, the split view controller’s implementation of this method calls show(_:sender:) instead.

The default implementation of this method calls the targetViewController(forAction:sender:) method to locate an object in the view controller hierarchy that overrides this method. It then calls the method on that target object, which displays the view controller in an appropriate way. If the targetViewController(forAction:sender:) method returns `nil`, this method uses the window’s root view controller to present `vc` modally.

You can override this method in custom view controllers to display `vc` yourself. Use this method to display `vc` in a secondary context. For example, a container view controller might use this method to replace its secondary child. Your implementation should adapt its behavior for both regular and compact environments.

## See Also

### Presenting a view controller

func show(UIViewController, sender: Any?)

Presents a view controller in a primary context.

func present(UIViewController, animated: Bool, completion: (() -> Void)?)

Presents a view controller modally.

func dismiss(animated: Bool, completion: (() -> Void)?)

Dismisses the view controller that was presented modally by the view controller.

var modalPresentationStyle: UIModalPresentationStyle

The presentation style for modal view controllers.

enum UIModalPresentationStyle

Modal presentation styles available when presenting view controllers.

var modalTransitionStyle: UIModalTransitionStyle

The transition style to use when presenting the view controller.

enum UIModalTransitionStyle

Transition styles available when presenting view controllers.

var isModalInPresentation: Bool

A Boolean value indicating whether the view controller enforces a modal behavior.

var definesPresentationContext: Bool

A Boolean value that indicates whether this view controller’s view is covered when the view controller or one of its descendants presents a view controller.

var providesPresentationContextTransitionStyle: Bool

A Boolean value that indicates whether the view controller specifies the transition style for view controllers it presents.

var disablesAutomaticKeyboardDismissal: Bool

Returns a Boolean indicating whether the current input view is dismissed automatically when changing controls.

class let showDetailTargetDidChangeNotification: NSNotification.Name

Posted when a split view controller is expanded or collapsed.

