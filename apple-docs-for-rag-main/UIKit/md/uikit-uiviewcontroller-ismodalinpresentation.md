

- UIKit
- UIViewController
-  isModalInPresentation 

Instance Property

# isModalInPresentation

A Boolean value indicating whether the view controller enforces a modal behavior.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var isModalInPresentation: Bool { get set }
```

## Discussion

The default value of this property is false. When you set it to true, UIKit ignores events outside the view controller’s bounds and prevents the interactive dismissal of the view controller while it is onscreen.

## See Also

### Related Documentation

Disabling the pull-down gesture for a sheet

Ensure a positive user experience when presenting a view controller as a sheet.

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

var definesPresentationContext: Bool

A Boolean value that indicates whether this view controller’s view is covered when the view controller or one of its descendants presents a view controller.

var providesPresentationContextTransitionStyle: Bool

A Boolean value that indicates whether the view controller specifies the transition style for view controllers it presents.

var disablesAutomaticKeyboardDismissal: Bool

Returns a Boolean indicating whether the current input view is dismissed automatically when changing controls.

class let showDetailTargetDidChangeNotification: NSNotification.Name

Posted when a split view controller is expanded or collapsed.

