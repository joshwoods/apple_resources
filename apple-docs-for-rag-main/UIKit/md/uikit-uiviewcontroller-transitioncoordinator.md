

- UIKit
- UIViewController
-  transitionCoordinator 

Instance Property

# transitionCoordinator

Returns the active transition coordinator object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var transitionCoordinator: (any UIViewControllerTransitionCoordinator)? { get }
```

## Return Value

The transition coordinator object associated with a currently active transition or `nil` if no transition is in progress.

## Discussion

When a presentation or dismissal is in progress, this method returns the transition coordinator object associated with that transition. If there is no in-progress transition associated with the current view controller, UIKit checks the view controller’s ancestors for a transition coordinator object and returns that object if it exists. You can use this object to create additional animations and synchronize them with the transition animations.

Container view controllers can override this method but in most cases should not need to. If you do override this method, first call `super` to see if there is an appropriate transition coordinator to return, and, if there is, return it.

For more information about the role of transition coordinators, see UIViewControllerTransitionCoordinator.

## See Also

### Adding a custom transition or presentation

var transitioningDelegate: (any UIViewControllerTransitioningDelegate)?

The delegate object that provides transition animator, interactive controller, and custom presentation controller objects.

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

