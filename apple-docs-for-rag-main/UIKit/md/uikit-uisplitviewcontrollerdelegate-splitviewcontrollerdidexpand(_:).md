

- UIKit
- UISplitViewControllerDelegate
-  splitViewControllerDidExpand(\_:) 

Instance Method

# splitViewControllerDidExpand(\_:)

Tells the delegate that the split view controller interface has expanded.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
optional func splitViewControllerDidExpand(_ svc: UISplitViewController)
```

## Parameters 

`svc`  

The split view controller whose interface has expanded.

## Discussion

This delegate method only applies to column-style split view interfaces. For more information, see Split view styles.

The split view controller calls this method after its interface has expanded, meaning that isCollapsed is false. Use this method to perform any customization associated with the expanded interface.

## See Also

### Expanding the interface

func splitViewController(UISplitViewController, displayModeForExpandingToProposedDisplayMode: UISplitViewController.DisplayMode) -> UISplitViewController.DisplayMode

Asks the delegate to provide the display mode to use after the split view interface expands.

func splitViewController(UISplitViewController, willShow: UISplitViewController.Column)

Tells the delegate that the specified column is about to be shown.

