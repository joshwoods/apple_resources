

- UIKit
- UITableViewDelegate
-  tableView(\_:didHighlightRowAt:) 

Instance Method

# tableView(\_:didHighlightRowAt:)

Tells the delegate that the specified row was highlighted.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    didHighlightRowAt indexPath: IndexPath
)
```

## Parameters 

`tableView`  

The table view that highlighted the cell.

`indexPath`  

The index path of the row that was highlighted.

## See Also

### Managing table view highlights

func tableView(UITableView, shouldHighlightRowAt: IndexPath) -> Bool

Asks the delegate if the specified row should be highlighted.

func tableView(UITableView, didUnhighlightRowAt: IndexPath)

Tells the delegate that the highlight was removed from the row at the specified index path.

