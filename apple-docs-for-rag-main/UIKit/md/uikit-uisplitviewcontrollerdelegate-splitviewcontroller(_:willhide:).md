

- UIKit
- UISplitViewControllerDelegate
-  splitViewController(\_:willHide:) 

Instance Method

# splitViewController(\_:willHide:)

Tells the delegate that the specified column is about to be hidden.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
optional func splitViewController(
    _ svc: UISplitViewController,
    willHide column: UISplitViewController.Column
)
```

## Parameters 

`svc`  

The split view controller whose column is being hidden.

`column`  

The column to be hidden. See UISplitViewController.Column for possible values.

## Discussion

This delegate method only applies to column-style split view interfaces. For more information, see Split view styles.

The split view controller calls this method when one of its columns is about to be hidden, for example with hide(_:). Use this method to perform any customization associated with hiding the column. You can use the split view controller’s transitionCoordinator to coordinate any of your animations alongside the transition animation.

## See Also

### Collapsing the interface

func splitViewController(UISplitViewController, topColumnForCollapsingToProposedTopColumn: UISplitViewController.Column) -> UISplitViewController.Column

Asks the delegate to provide the column to display after the split view interface collapses.

func splitViewControllerDidCollapse(UISplitViewController)

Tells the delegate that the split view controller interface has collapsed.

