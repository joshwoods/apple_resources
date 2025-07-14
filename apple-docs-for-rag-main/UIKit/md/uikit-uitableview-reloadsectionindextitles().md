

- UIKit
- UITableView
-  reloadSectionIndexTitles() 

Instance Method

# reloadSectionIndexTitles()

Reloads the items in the index bar along the right side of the table view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func reloadSectionIndexTitles()
```

## Discussion

This method gives you a way to update the section index after inserting or deleting sections without having to reload the whole table.

## See Also

### Related Documentation

func sectionIndexTitles(for: UITableView) -> [String]?

Asks the data source to return the titles for the sections of a table view.

### Reloading the table view

var hasUncommittedUpdates: Bool

A Boolean value that indicates whether the table view’s appearance contains changes that aren’t present in its data source.

func reconfigureRows(at: [IndexPath])

Updates the data for the rows at the index paths you specify, preserving the existing cells for the rows.

func reloadData()

Reloads the rows and sections of the table view.

func reloadRows(at: [IndexPath], with: UITableView.RowAnimation)

Reloads the specified rows using the provided animation effect.

func reloadSections(IndexSet, with: UITableView.RowAnimation)

Reloads the specified sections using the provided animation effect.

