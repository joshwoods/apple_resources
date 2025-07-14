

- UIKit
- UITableView
-  reloadRows(at:with:) 

Instance Method

# reloadRows(at:with:)

Reloads the specified rows using the provided animation effect.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func reloadRows(
    at indexPaths: [IndexPath],
    with animation: UITableView.RowAnimation
)
```

## Parameters 

`indexPaths`  

An array of NSIndexPath objects identifying the rows to reload.

`animation`  

A constant that indicates how the reloading is to be animated, for example, fade out or slide out from the bottom. See UITableView.RowAnimation for descriptions of these constants.

The animation constant affects the direction in which both the old and the new rows slide. For example, if the animation constant is UITableView.RowAnimation.right, the old rows slide out to the right and the new cells slide in from the right.

## Discussion

Reloading a row causes the table view to ask its data source for a new cell for that row. The table animates that new cell in as it animates the old row out. Call this method if you want to alert the user that the value of a cell is changing. If, however, notifying the user isn’t important — that is, you just want to change the value that a cell is displaying — you can get the cell for a particular row and set its new value.

When this method is called in an animation block defined by the beginUpdates() and endUpdates() methods, it behaves similarly to deleteRows(at:with:). The indexes that UITableView passes to the method are specified in the state of the table view prior to any updates. This happens regardless of ordering of the insertion, deletion, and reloading method calls within the animation block.

## See Also

### Related Documentation

func insertRows(at: [IndexPath], with: UITableView.RowAnimation)

Inserts rows in the table view at the locations that an array of index paths identifies, with an option to animate the insertion.

### Reloading the table view

var hasUncommittedUpdates: Bool

A Boolean value that indicates whether the table view’s appearance contains changes that aren’t present in its data source.

func reconfigureRows(at: [IndexPath])

Updates the data for the rows at the index paths you specify, preserving the existing cells for the rows.

func reloadData()

Reloads the rows and sections of the table view.

func reloadSections(IndexSet, with: UITableView.RowAnimation)

Reloads the specified sections using the provided animation effect.

func reloadSectionIndexTitles()

Reloads the items in the index bar along the right side of the table view.

