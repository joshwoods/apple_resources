

- UIKit
-  UISplitViewControllerDelegate 

Protocol

# UISplitViewControllerDelegate

The methods adopted by the object you use to manage changes to a split view interface.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UISplitViewControllerDelegate
```

## Overview

Use the methods of this protocol to respond to changes in the current display mode and to the current interface orientation. When the split view interface collapses and expands, or when a new view controller is added to the interface, you can also use these methods to configure the child view controllers.

The methods of this protocol are all optional. If you don’t implement any of the methods, the split view controller provides default behavior to handle the collapsing and expanding transitions.

For more information, see UISplitViewController.

### Column-style split views

In a column-style split view interface, you use these delegate methods to customize interface transition behavior:

- splitViewController(_:topColumnForCollapsingToProposedTopColumn:)

- splitViewController(_:willHide:)

- splitViewControllerDidCollapse(_:)

- splitViewController(_:displayModeForExpandingToProposedDisplayMode:)

- splitViewController(_:willShow:)

- splitViewControllerDidExpand(_:)

### Classic split views

In a classic split view interface, you use these delegate methods to customize interface transition behavior:

- primaryViewController(forCollapsing:)

- splitViewController(_:collapseSecondary:onto:)

- primaryViewController(forExpanding:)

- splitViewController(_:separateSecondaryFrom:)

- splitViewController(_:show:sender:)

- splitViewController(_:showDetail:sender:)

At the end of a collapse transition, the split view controller typically shows only the content from its primary view controller. You can change this behavior by implementing the primaryViewController(forCollapsing:) method in your split view controller delegate. You might use that method to specify the secondary view controller or an entirely different view controller—perhaps one better suited for display in a horizontally compact environment.

If you want to perform any additional adjustments of the view controllers and view hierarchy, you can also implement the splitViewController(_:collapseSecondary:onto:) method in your delegate.

The expansion process reverses the collapsing process by asking the delegate to designate which view controller becomes the primary view controller and to give the delegate a chance to perform the transition itself. If you implement the delegate methods for collapsing your split view interface, you should also implement the primaryViewController(forExpanding:) and splitViewController(_:separateSecondaryFrom:) methods for expanding that interface.

## Topics

### Specifying the interface orientations

func splitViewControllerPreferredInterfaceOrientationForPresentation(UISplitViewController) -> UIInterfaceOrientation

Asks the delegate for the orientation to use when presenting the split view controller.

func splitViewControllerSupportedInterfaceOrientations(UISplitViewController) -> UIInterfaceOrientationMask

Asks the delegate to specify the interface orientations that the split view controller supports.

### Responding to display mode changes

func splitViewController(UISplitViewController, willChangeTo: UISplitViewController.DisplayMode)

Tells the delegate that the display mode for the split view controller is about to change.

func targetDisplayModeForAction(in: UISplitViewController) -> UISplitViewController.DisplayMode

Asks the delegate to provide the display mode to apply when a split view controller action occurs.

### Collapsing the interface

func splitViewController(UISplitViewController, topColumnForCollapsingToProposedTopColumn: UISplitViewController.Column) -> UISplitViewController.Column

Asks the delegate to provide the column to display after the split view interface collapses.

func splitViewController(UISplitViewController, willHide: UISplitViewController.Column)

Tells the delegate that the specified column is about to be hidden.

func splitViewControllerDidCollapse(UISplitViewController)

Tells the delegate that the split view controller interface has collapsed.

### Expanding the interface

func splitViewController(UISplitViewController, displayModeForExpandingToProposedDisplayMode: UISplitViewController.DisplayMode) -> UISplitViewController.DisplayMode

Asks the delegate to provide the display mode to use after the split view interface expands.

func splitViewController(UISplitViewController, willShow: UISplitViewController.Column)

Tells the delegate that the specified column is about to be shown.

func splitViewControllerDidExpand(UISplitViewController)

Tells the delegate that the split view controller interface has expanded.

### Handling the presentation gesture

func splitViewControllerInteractivePresentationGestureWillBegin(UISplitViewController)

Tells the delegate that the interactive presentation gesture is about to begin.

func splitViewControllerInteractivePresentationGestureDidEnd(UISplitViewController)

Tells the delegate when the interactive presentation gesture ends.

### Collapsing and expanding classic split views

func primaryViewController(forCollapsing: UISplitViewController) -> UIViewController?

Asks the delegate to provide the single view controller to display after the split view interface collapses.

func splitViewController(UISplitViewController, collapseSecondary: UIViewController, onto: UIViewController) -> Bool

Asks the delegate to adjust the primary view controller and to incorporate the secondary view controller into the collapsed interface.

func primaryViewController(forExpanding: UISplitViewController) -> UIViewController?

Asks the delegate to provide the view controller to display in the primary position when the split view interface expands.

func splitViewController(UISplitViewController, separateSecondaryFrom: UIViewController) -> UIViewController?

Asks the delegate to provide the new secondary view controller for the split view interface.

### Overriding the presentation behavior

func splitViewController(UISplitViewController, show: UIViewController, sender: Any?) -> Bool

Asks the delegate if it will do the work of displaying a view controller in the primary position of the split view interface.

func splitViewController(UISplitViewController, showDetail: UIViewController, sender: Any?) -> Bool

Asks the delegate if it will do the work of displaying a view controller in the secondary position of the split view interface.

### Deprecated methods

func splitViewController(UISplitViewController, shouldHide: UIViewController, in: UIInterfaceOrientation) -> Bool

Asks the delegate whether the first view controller should be hidden for the specified orientation.

Deprecated

func splitViewController(UISplitViewController, willHide: UIViewController, with: UIBarButtonItem, for: UIPopoverController)

Tells the delegate that the specified view controller is about to be hidden.

Deprecated

func splitViewController(UISplitViewController, willShow: UIViewController, invalidating: UIBarButtonItem)

Tells the delegate that the specified view controller is about to be shown again.

Deprecated

func splitViewController(UISplitViewController, popoverController: UIPopoverController, willPresent: UIViewController)

Tells the delegate that the hidden view controller is about to be displayed in a popover.

Deprecated

## See Also

### Customizing the split view transitions

var delegate: (any UISplitViewControllerDelegate)?

The delegate you use to manage changes to a split view interface.

