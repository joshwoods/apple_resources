

- UIKit
- UITableView
-  footerView(forSection:) 

Instance Method

# footerView(forSection:)

Returns the footer view for the specified section.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func footerView(forSection section: Int) -> UITableViewHeaderFooterView?
```

## Parameters 

`section`  

An index number that identifies a section of the table. Table views in a plain style have a section index of zero.

## Return Value

The footer view associated with the section, or `nil` if the section does not have a footer view.

## See Also

### Getting cells and section-based views

func cellForRow(at: IndexPath) -> UITableViewCell?

Returns the table cell at the index path you specify.

func headerView(forSection: Int) -> UITableViewHeaderFooterView?

Returns the header view for the specified section.

func indexPath(for: UITableViewCell) -> IndexPath?

Returns an index path that represents the row and section of a specified table-view cell.

func indexPathForRow(at: CGPoint) -> IndexPath?

Returns an index path that identifies the row and section at the specified point.

func indexPathsForRows(in: CGRect) -> [IndexPath]?

Returns an array of index paths, each representing a row that the specified rectangle encloses.

var visibleCells: [UITableViewCell]

The table cells that are visible in the table view.

var indexPathsForVisibleRows: [IndexPath]?

An array of index paths, each identifying a visible row in the table view.

