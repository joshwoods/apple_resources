

- UIKit
- UITableView
-  hasUncommittedUpdates 

Instance Property

# hasUncommittedUpdates

A Boolean value that indicates whether the table view’s appearance contains changes that aren’t present in its data source.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var hasUncommittedUpdates: Bool { get }
```

## Discussion

The value of this property is true when the table view contains placeholder cells or is handling a drop and is in the middle of reordering its rows. When this property is true, avoid making any significant changes to the table view. Specifically, don’t call reloadData(), which forces the table to delete any uncommitted changes before retrieving fresh data from the data source object.

## See Also

### Reloading the table view

func reconfigureRows(at: [IndexPath])

Updates the data for the rows at the index paths you specify, preserving the existing cells for the rows.

func reloadData()

Reloads the rows and sections of the table view.

func reloadRows(at: [IndexPath], with: UITableView.RowAnimation)

Reloads the specified rows using the provided animation effect.

func reloadSections(IndexSet, with: UITableView.RowAnimation)

Reloads the specified sections using the provided animation effect.

func reloadSectionIndexTitles()

Reloads the items in the index bar along the right side of the table view.

