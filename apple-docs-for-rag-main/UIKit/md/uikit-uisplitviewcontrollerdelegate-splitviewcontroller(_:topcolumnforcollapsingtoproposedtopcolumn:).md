

- UIKit
- UISplitViewControllerDelegate
-  splitViewController(\_:topColumnForCollapsingToProposedTopColumn:) 

Instance Method

# splitViewController(\_:topColumnForCollapsingToProposedTopColumn:)

Asks the delegate to provide the column to display after the split view interface collapses.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
optional func splitViewController(
    _ svc: UISplitViewController,
    topColumnForCollapsingToProposedTopColumn proposedTopColumn: UISplitViewController.Column
) -> UISplitViewController.Column
```

## Parameters 

`svc`  

The split view controller whose interface is collapsing.

`proposedTopColumn`  

The proposed column to display in the collapsed interface.

## Return Value

The column corresponding to the view controller to display in the collapsed interface. This value may be the same as `proposedTopColumn`, or you may return a different value.

## Discussion

This delegate method only applies to column-style split view interfaces. For more information, see Split view styles.

When the split view controller transitions from a horizontally regular to a horizontally compact size class, it calls this method and asks you for the column to display when that transition is complete. Use this method to customize the view controller you’re collapsing to. For example, you might use this opportunity to configure the interface in the view controller associated with the UISplitViewController.Column.compact column before returning that column.

## See Also

### Collapsing the interface

func splitViewController(UISplitViewController, willHide: UISplitViewController.Column)

Tells the delegate that the specified column is about to be hidden.

func splitViewControllerDidCollapse(UISplitViewController)

Tells the delegate that the split view controller interface has collapsed.

