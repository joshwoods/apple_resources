

- AppKit
- NSTableView
-  didRemove(\_:forRow:) 

Instance Method

# didRemove(\_:forRow:)

Invoked when a row view is removed from the table.

macOS 10.7+

``` source
@MainActor
func didRemove(
    _ rowView: NSTableRowView,
    forRow row: Int
)
```

## Parameters 

`rowView`  

The row view.

`row`  

The row index. The index is `-1` for rows that are being deleted from the table, and no longer have a valid row; otherwise it is the valid row that is being removed due to it being moved off screen.

## Discussion

The subclass can implement this method to be alerted when `rowView` has been removed from the table. The removed `rowView` may be reused by the table, so any additionally inserted views should be removed at this point. Subclasses must be sure to call `super`.

Note

This method is only applicable to NSView-based table views.

## See Also

### Adding and Deleting Row Views

func didAdd(NSTableRowView, forRow: Int)

Invoked when a row view is added to the table.

