

- UIKit
- UIViewController
-  modalTransitionStyle 

Instance Property

# modalTransitionStyle

The transition style to use when presenting the view controller.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var modalTransitionStyle: UIModalTransitionStyle { get set }
```

## Discussion

This property determines how the view controller’s is animated onscreen when it is presented using the present(_:animated:completion:) method. To change the transition type, you must set this property before presenting the view controller. The default value for this property is UIModalTransitionStyle.coverVertical.

For a list of possible transition styles, and their compatibility with the available presentation styles, see the UIModalTransitionStyle constant descriptions.

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

