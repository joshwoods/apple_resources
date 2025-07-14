

- UIKit
- UISplitViewController
-  show(\_:) 

Instance Method

# show(\_:)

Presents the view controller in the specified column of the split view interface.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
func show(_ column: UISplitViewController.Column)
```

## Parameters 

`column`  

The corresponding column of the split view interface to show. See UISplitViewController.Column for values.

## Discussion

When you call this method, the split view interface transitions to the closest display mode available for the current split behavior where the specified column is fully visible.

The split view controller chooses the appropriate transition to display the view controller in the specified column. For example, calling this method with UISplitViewController.Column.secondary when the split behavior is UISplitViewController.SplitBehavior.displace changes the display mode from UISplitViewController.DisplayMode.twoDisplaceSecondary to UISplitViewController.DisplayMode.oneBesideSecondary, which hides the primary column to show the unobstructed secondary column.

After you call this method, you can use the split view controller’s transitionCoordinator to coordinate any of your animations alongside the transition animation.

## See Also

### Displaying the child view controllers

func hide(UISplitViewController.Column)

Dismisses the view controller in the specified column of the split view interface.

func show(UIViewController, sender: Any?)

Presents the specified view controller as the primary view controller in the split view interface.

func showDetailViewController(UIViewController, sender: Any?)

Presents the specified view controller as the secondary view controller of the split view interface.

