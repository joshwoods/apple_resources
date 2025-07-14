

- UIKit
- UIViewController
-  transitioningDelegate 

Instance Property

# transitioningDelegate

The delegate object that provides transition animator, interactive controller, and custom presentation controller objects.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var transitioningDelegate: (any UIViewControllerTransitioningDelegate)? { get set }
```

## Discussion

When the view controller’s modalPresentationStyle property is UIModalPresentationStyle.custom, UIKit uses the object in this property to facilitate transitions and presentations for the view controller. The transitioning delegate object is a custom object that you provide and that conforms to the UIViewControllerTransitioningDelegate protocol. Its job is to vend the animator objects used to animate this view controller’s view onscreen and an optional presentation controller to provide any additional chrome and animations.

## See Also

### Adding a custom transition or presentation

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

var restoresFocusAfterTransition: Bool

A Boolean value that indicates whether an item that previously was focused should again become focused when the item’s view controller becomes visible and focusable.

Customizing and resizing sheets in UIKit

Discover how to create a layered and customized sheet experience in UIKit.

