

- UIKit
- UIViewController
-  modalPresentationStyle 

Instance Property

# modalPresentationStyle

The presentation style for modal view controllers.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var modalPresentationStyle: UIModalPresentationStyle { get set }
```

## Discussion

Presentation style defines how the system presents a modal view controller. The system uses this value only in regular-width size classes. In compact-width size classes, some styles take on the behavior of other styles. You can influence this behavior by implementing the adaptivePresentationStyle(for:traitCollection:) method.

Presentation style also impacts the content size of a modal view controller. For example, UIModalPresentationStyle.pageSheet uses an explicit size that the system provides. By contrast, UIModalPresentationStyle.formSheet uses the view controller’s preferredContentSize property, which you can set.

The default value is UIModalPresentationStyle.automatic. For a list of presentation styles and their compatibility with the various transition styles, see UIModalPresentationStyle.

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

