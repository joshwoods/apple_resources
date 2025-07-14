

- UIKit
- UIViewController
-  definesPresentationContext 

Instance Property

# definesPresentationContext

A Boolean value that indicates whether this view controller’s view is covered when the view controller or one of its descendants presents a view controller.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var definesPresentationContext: Bool { get set }
```

## Discussion

When using the UIModalPresentationStyle.currentContext or UIModalPresentationStyle.overCurrentContext style to present a view controller, this property controls which existing view controller in your view controller hierarchy is actually covered by the new content. When a context-based presentation occurs, UIKit starts at the presenting view controller and walks up the view controller hierarchy. If it finds a view controller whose value for this property is true, it asks that view controller to present the new view controller. If no view controller defines the presentation context, UIKit asks the window’s root view controller to handle the presentation.

The default value for this property is false. Some system-provided view controllers, such as UINavigationController, change the default value to true.

## See Also

### Presenting a view controller

func show(UIViewController, sender: Any?)

Presents a view controller in a primary context.

func showDetailViewController(UIViewController, sender: Any?)

Presents a view controller in a secondary (or detail) context.

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

var providesPresentationContextTransitionStyle: Bool

A Boolean value that indicates whether the view controller specifies the transition style for view controllers it presents.

var disablesAutomaticKeyboardDismissal: Bool

Returns a Boolean indicating whether the current input view is dismissed automatically when changing controls.

class let showDetailTargetDidChangeNotification: NSNotification.Name

Posted when a split view controller is expanded or collapsed.

