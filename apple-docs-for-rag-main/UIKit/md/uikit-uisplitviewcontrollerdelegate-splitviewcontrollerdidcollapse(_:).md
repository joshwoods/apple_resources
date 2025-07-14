

- UIKit
- UISplitViewControllerDelegate
-  splitViewControllerDidCollapse(\_:) 

Instance Method

# splitViewControllerDidCollapse(\_:)

Tells the delegate that the split view controller interface has collapsed.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
optional func splitViewControllerDidCollapse(_ svc: UISplitViewController)
```

## Parameters 

`svc`  

The split view controller whose interface has collapsed.

## Discussion

This delegate method only applies to column-style split view interfaces. For more information, see Split view styles.

The split view controller calls this method after its interface has collapsed, meaning that isCollapsed is true. Use this method to perform any customization associated with the collapsed interface.

## See Also

### Collapsing the interface

func splitViewController(UISplitViewController, topColumnForCollapsingToProposedTopColumn: UISplitViewController.Column) -> UISplitViewController.Column

Asks the delegate to provide the column to display after the split view interface collapses.

func splitViewController(UISplitViewController, willHide: UISplitViewController.Column)

Tells the delegate that the specified column is about to be hidden.

