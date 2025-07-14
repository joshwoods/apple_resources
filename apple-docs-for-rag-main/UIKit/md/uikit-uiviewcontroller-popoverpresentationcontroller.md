

- UIKit
- UIViewController
-  popoverPresentationController 

Instance Property

# popoverPresentationController

The nearest popover presentation controller that is managing the current view controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var popoverPresentationController: UIPopoverPresentationController? { get }
```

## Mentioned in 

Getting the user’s attention with alerts and action sheets

## Discussion

If the view controller or one of its ancestors is managed by a popover presentation controller, this property contains that object. This property is `nil` if the view controller is not managed by a popover presentation controller.

If you created the view controller but have not yet presented it, accessing this property creates a popover presentation controller when the value in the modalPresentationStyle property is UIModalPresentationStyle.popover. If the modal presentation style is a different value, this property is `nil`.

## See Also

### Adding a custom transition or presentation

var transitioningDelegate: (any UIViewControllerTransitioningDelegate)?

The delegate object that provides transition animator, interactive controller, and custom presentation controller objects.

var transitionCoordinator: (any UIViewControllerTransitionCoordinator)?

Returns the active transition coordinator object.

func targetViewController(forAction: Selector, sender: Any?) -> UIViewController?

Returns the view controller that responds to the action.

var presentationController: UIPresentationController?

The presentation controller that’s managing the current view controller.

var sheetPresentationController: UISheetPresentationController?

The sheet presentation controller for the view controller.

var activePresentationController: UIPresentationController?

The presentation controller that’s managing the view controller.

var restoresFocusAfterTransition: Bool

A Boolean value that indicates whether an item that previously was focused should again become focused when the item’s view controller becomes visible and focusable.

Customizing and resizing sheets in UIKit

Discover how to create a layered and customized sheet experience in UIKit.

