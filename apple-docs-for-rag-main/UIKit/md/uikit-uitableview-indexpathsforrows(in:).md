

- UIKit
- UITableView
-  indexPathsForRows(in:) 

Instance Method

# indexPathsForRows(in:)

Returns an array of index paths, each representing a row that the specified rectangle encloses.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func indexPathsForRows(in rect: CGRect) -> [IndexPath]?
```

## Parameters 

`rect`  

A rectangle defining an area of the table view in local coordinates.

## Return Value

An array of NSIndexPath objects each representing a row and section index identifying a row within `rect`. Returns an empty array if there aren’t any rows to return.

## See Also

### Getting cells and section-based views

func cellForRow(at: IndexPath) -> UITableViewCell?

Returns the table cell at the index path you specify.

func headerView(forSection: Int) -> UITableViewHeaderFooterView?

Returns the header view for the specified section.

func footerView(forSection: Int) -> UITableViewHeaderFooterView?

Returns the footer view for the specified section.

func indexPath(for: UITableViewCell) -> IndexPath?

Returns an index path that represents the row and section of a specified table-view cell.

func indexPathForRow(at: CGPoint) -> IndexPath?

Returns an index path that identifies the row and section at the specified point.

var visibleCells: [UITableViewCell]

The table cells that are visible in the table view.

var indexPathsForVisibleRows: [IndexPath]?

An array of index paths, each identifying a visible row in the table view.

