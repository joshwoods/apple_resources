

- UIKit
- UITableView
-  reloadData() 

Instance Method

# reloadData()

Reloads the rows and sections of the table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func reloadData()
```

## Discussion

Call this method to reload all the data that’s used to construct the table, including cells, section headers and footers, index arrays, and so on. For efficiency, the table view redisplays only those rows that are visible. It adjusts offsets if the table shrinks as a result of the reload. The table view’s delegate or data source calls this method when it wants the table view to completely reload its data. It shouldn’t be called in the methods that insert or delete rows, especially within an animation block implemented with calls to beginUpdates() and endUpdates().

Important

Don’t call this method when the hasUncommittedUpdates property is true. Doing so forces the table view to delete any uncommitted changes before reloading the data.

## See Also

### Reloading the table view

var hasUncommittedUpdates: Bool

A Boolean value that indicates whether the table view’s appearance contains changes that aren’t present in its data source.

func reconfigureRows(at: [IndexPath])

Updates the data for the rows at the index paths you specify, preserving the existing cells for the rows.

func reloadRows(at: [IndexPath], with: UITableView.RowAnimation)

Reloads the specified rows using the provided animation effect.

func reloadSections(IndexSet, with: UITableView.RowAnimation)

Reloads the specified sections using the provided animation effect.

func reloadSectionIndexTitles()

Reloads the items in the index bar along the right side of the table view.

