

- AppKit
- NSTableViewDelegate
-  tableView(\_:shouldReorderColumn:toColumn:) 

Instance Method

# tableView(\_:shouldReorderColumn:toColumn:)

Asks the delegate to allow or prohibit the specified column to be dragged to a new location.

macOS 10.6+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    shouldReorderColumn columnIndex: Int,
    toColumn newColumnIndex: Int
) -> Bool
```

## Parameters 

`tableView`  

The table view that sent the message.

`columnIndex`  

The index of the column being dragged.

`newColumnIndex`  

The proposed target index of the column.

## Return Value

true if the column reordering should be allowed, otherwise false.

## Discussion

When a column is initially dragged by the user, the delegate is first called with a `newColumnIndex` value of `-1`. Returning false will disallow that column from being reordered at all. Returning true allows it to be reordered, and the delegate will be called again when the column reaches a new location.

The actual NSTableColumn instance can be retrieved from the tableColumns array.

If this method isn’t implemented, all columns are considered reorderable.

## See Also

### Moving and resizing columns

func tableView(NSTableView, didDrag: NSTableColumn)

Tells the delegate that the specified table column was dragged.

func tableViewColumnDidMove(Notification)

Tells the delegate that a table column was moved by user action.

func tableViewColumnDidResize(Notification)

Tells the delegate that a table column was resized.

