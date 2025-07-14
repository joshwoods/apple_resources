

- UIKit
- UIViewController
-  restoresFocusAfterTransition 

Instance Property

# restoresFocusAfterTransition

A Boolean value that indicates whether an item that previously was focused should again become focused when the item’s view controller becomes visible and focusable.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var restoresFocusAfterTransition: Bool { get set }
```

## Discussion

When the value of this property is true, the item that was last focused automatically becomes focused when its view controller becomes visible and focusable. For example, if an item in the view controller is focused and a second view controller is presented, the original item becomes focused again when the second view controller is dismissed. The default value of this property is true.

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

var popoverPresentationController: UIPopoverPresentationController?

The nearest popover presentation controller that is managing the current view controller.

var sheetPresentationController: UISheetPresentationController?

The sheet presentation controller for the view controller.

var activePresentationController: UIPresentationController?

The presentation controller that’s managing the view controller.

Customizing and resizing sheets in UIKit

Discover how to create a layered and customized sheet experience in UIKit.

