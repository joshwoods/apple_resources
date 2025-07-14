

- UIKit
- UIViewController
-  present(\_:animated:completion:) 

Instance Method

# present(\_:animated:completion:)

Presents a view controller modally.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func present(
    _ viewControllerToPresent: UIViewController,
    animated flag: Bool,
    completion: (() -> Void)? = nil
)
```

## Parameters 

`viewControllerToPresent`  

The view controller to display over the current view controller’s content.

`flag`  

Pass true to animate the presentation; otherwise, pass false.

`completion`  

The block to execute after the presentation finishes. This block has no return value and takes no parameters. You may specify `nil` for this parameter.

## Mentioned in 

Providing access to directories

Getting the user’s attention with alerts and action sheets

Presenting selected documents

Displaying transient content in a popover

## Discussion

In a horizontally regular environment, the view controller is presented in the style specified by the modalPresentationStyle property. In a horizontally compact environment, the view controller is presented full screen by default. If you associate an adaptive delegate with the presentation controller associated with the object in `viewControllerToPresent`, you can modify the presentation style dynamically.

The object on which you call this method may not always be the one that handles the presentation. Each presentation style has different rules governing its behavior. For example, a full-screen presentation must be made by a view controller that itself covers the entire screen. If the current view controller is unable to fulfill a request, it forwards the request up the view controller hierarchy to its nearest parent, which can then handle or forward the request.

Before displaying the view controller, this method resizes the presented view controller’s view based on the presentation style. For most presentation styles, the resulting view is then animated onscreen using the transition style in the modalTransitionStyle property of the presented view controller. For custom presentations, the view is animated onscreen using the presented view controller’s transitioning delegate. For current context presentations, the view may be animated onscreen using the current view controller’s transition style.

The completion handler is called after the viewDidAppear(_:) method is called on the presented view controller.

## See Also

### Related Documentation

var presentedViewController: UIViewController?

The view controller that is presented by this view controller, or one of its ancestors in the view controller hierarchy.

var presentingViewController: UIViewController?

The view controller that presented this view controller.

### Presenting a view controller

func show(UIViewController, sender: Any?)

Presents a view controller in a primary context.

func showDetailViewController(UIViewController, sender: Any?)

Presents a view controller in a secondary (or detail) context.

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

