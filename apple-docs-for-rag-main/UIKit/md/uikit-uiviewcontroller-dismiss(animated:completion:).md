

- UIKit
- UIViewController
-  dismiss(animated:completion:) 

Instance Method

# dismiss(animated:completion:)

Dismisses the view controller that was presented modally by the view controller.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func dismiss(
    animated flag: Bool,
    completion: (() -> Void)? = nil
)
```

## Parameters 

`flag`  

Pass true to animate the transition.

`completion`  

The block to execute after the view controller is dismissed. This block has no return value and takes no parameters. You may specify `nil` for this parameter.

## Discussion

The presenting view controller is responsible for dismissing the view controller it presented. If you call this method on the presented view controller itself, UIKit asks the presenting view controller to handle the dismissal.

If you present several view controllers in succession, thus building a stack of presented view controllers, calling this method on a view controller lower in the stack dismisses its immediate child view controller and all view controllers above that child on the stack. When this happens, only the top-most view is dismissed in an animated fashion; any intermediate view controllers are simply removed from the stack. The top-most view is dismissed using its modal transition style, which may differ from the styles used by other view controllers lower in the stack.

If you want to retain a reference to the view controller’s presented view controller, get the value in the presentedViewController property before calling this method.

The completion handler is called after the viewDidDisappear(_:) method is called on the presented view controller.

## See Also

### Presenting a view controller

func show(UIViewController, sender: Any?)

Presents a view controller in a primary context.

func showDetailViewController(UIViewController, sender: Any?)

Presents a view controller in a secondary (or detail) context.

func present(UIViewController, animated: Bool, completion: (() -> Void)?)

Presents a view controller modally.

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

