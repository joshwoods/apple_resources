

- UIKit
- UITableView
-  indexPathForRow(at:) 

Instance Method

# indexPathForRow(at:)

Returns an index path that identifies the row and section at the specified point.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func indexPathForRow(at point: CGPoint) -> IndexPath?
```

## Parameters 

`point`  

A point in the local coordinate system of the table view (the table view’s bounds).

## Return Value

An index path representing the row and section associated with `point`, or `nil` if the point is out of the bounds of any row.

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

func indexPathsForRows(in: CGRect) -> [IndexPath]?

Returns an array of index paths, each representing a row that the specified rectangle encloses.

var visibleCells: [UITableViewCell]

The table cells that are visible in the table view.

var indexPathsForVisibleRows: [IndexPath]?

An array of index paths, each identifying a visible row in the table view.

