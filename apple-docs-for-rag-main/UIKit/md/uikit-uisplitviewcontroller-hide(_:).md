

- UIKit
- UISplitViewController
-  hide(\_:) 

Instance Method

# hide(\_:)

Dismisses the view controller in the specified column of the split view interface.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
func hide(_ column: UISplitViewController.Column)
```

## Parameters 

`column`  

The corresponding column of the split view interface to hide. See UISplitViewController.Column for values.

## Discussion

When you call this method, the split view interface transitions to the closest display mode available for the current split behavior where the specified column is hidden.

This method does not support hiding the UISplitViewController.Column.secondary column.

After you call this method, you can use the split view controller’s transitionCoordinator to coordinate any of your animations alongside the transition animation.

## See Also

### Displaying the child view controllers

func show(UISplitViewController.Column)

Presents the view controller in the specified column of the split view interface.

func show(UIViewController, sender: Any?)

Presents the specified view controller as the primary view controller in the split view interface.

func showDetailViewController(UIViewController, sender: Any?)

Presents the specified view controller as the secondary view controller of the split view interface.

