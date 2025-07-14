

- UIKit
- UIViewController
-  showDetailTargetDidChangeNotification 

Type Property

# showDetailTargetDidChangeNotification

Posted when a split view controller is expanded or collapsed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
class let showDetailTargetDidChangeNotification: NSNotification.Name
```

## Discussion

When a view controller is using show(_:sender:) or showDetailViewController(_:sender:), it may need to know when a split view controller higher in the view hierarchy has changed. This notification is sent when a split view controller expands or collapses. The object of this notification is the view controller that caused the change.

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

var definesPresentationContext: Bool

A Boolean value that indicates whether this view controller’s view is covered when the view controller or one of its descendants presents a view controller.

var providesPresentationContextTransitionStyle: Bool

A Boolean value that indicates whether the view controller specifies the transition style for view controllers it presents.

var disablesAutomaticKeyboardDismissal: Bool

Returns a Boolean indicating whether the current input view is dismissed automatically when changing controls.

