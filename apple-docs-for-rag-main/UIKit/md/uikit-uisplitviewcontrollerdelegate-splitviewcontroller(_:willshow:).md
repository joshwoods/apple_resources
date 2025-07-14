

- UIKit
- UISplitViewControllerDelegate
-  splitViewController(\_:willShow:) 

Instance Method

# splitViewController(\_:willShow:)

Tells the delegate that the specified column is about to be shown.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
optional func splitViewController(
    _ svc: UISplitViewController,
    willShow column: UISplitViewController.Column
)
```

## Parameters 

`svc`  

The split view controller whose column is being shown.

`column`  

The column to be shown. See UISplitViewController.Column for possible values.

## Discussion

This delegate method only applies to column-style split view interfaces. For more information, see Split view styles.

The split view controller calls this method when one of its columns is about to be shown, for example with show(_:). Use this method to perform any customization associated with showing the column. You can use the split view controller’s transitionCoordinator to coordinate any of your animations alongside the transition animation.

## See Also

### Expanding the interface

func splitViewController(UISplitViewController, displayModeForExpandingToProposedDisplayMode: UISplitViewController.DisplayMode) -> UISplitViewController.DisplayMode

Asks the delegate to provide the display mode to use after the split view interface expands.

func splitViewControllerDidExpand(UISplitViewController)

Tells the delegate that the split view controller interface has expanded.

