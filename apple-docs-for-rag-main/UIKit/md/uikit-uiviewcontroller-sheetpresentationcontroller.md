

- UIKit
- UIViewController
-  sheetPresentationController 

Instance Property

# sheetPresentationController

The sheet presentation controller for the view controller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var sheetPresentationController: UISheetPresentationController? { get }
```

## Discussion

If modalPresentationStyle is UIModalPresentationStyle.pageSheet or UIModalPresentationStyle.formSheet, this property contains a sheet presentation controller instance. Access this instance to customize or adjust the sheet before or after it presents.

If modalPresentationStyle has a value other than UIModalPresentationStyle.pageSheet or UIModalPresentationStyle.formSheet, the value of this property is `nil`.

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

var activePresentationController: UIPresentationController?

The presentation controller that’s managing the view controller.

var restoresFocusAfterTransition: Bool

A Boolean value that indicates whether an item that previously was focused should again become focused when the item’s view controller becomes visible and focusable.

Customizing and resizing sheets in UIKit

Discover how to create a layered and customized sheet experience in UIKit.

