

- UIKit
- UITableViewDelegate
-  tableView(\_:didUnhighlightRowAt:) 

Instance Method

# tableView(\_:didUnhighlightRowAt:)

Tells the delegate that the highlight was removed from the row at the specified index path.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    didUnhighlightRowAt indexPath: IndexPath
)
```

## Parameters 

`tableView`  

The table view that removed the highlight from the cell.

`indexPath`  

The index path of the row that had its highlight removed.

## See Also

### Managing table view highlights

func tableView(UITableView, shouldHighlightRowAt: IndexPath) -> Bool

Asks the delegate if the specified row should be highlighted.

func tableView(UITableView, didHighlightRowAt: IndexPath)

Tells the delegate that the specified row was highlighted.

