

- AppKit
- NSTableView
-  hideRows(at:withAnimation:) 

Instance Method

# hideRows(at:withAnimation:)

Hides the specified table rows.

macOS 10.11+

``` source
@MainActor
func hideRows(
    at indexes: IndexSet,
    withAnimation rowAnimation: NSTableView.AnimationOptions = []
)
```

## Parameters 

`indexes`  

An index set containing indexes of the rows to be hidden.

`rowAnimation`  

An animation effect to be applied when the rows are hidden.

## Discussion

Use this method when you no longer want the data to be visible to the user, but you don’t want to permanently remove the data. Hidden table rows have a height of zero and cannot be selected by the user. However, if a selected table row is hidden, it will remain selected.

Hiding a table row causes the tableView(_:didRemove:forRow:) delegate method to be invoked.

## See Also

### Related Documentation

struct AnimationOptions

Specifies the animation effects to apply when inserting or removing rows.

func tableView(NSTableView, didRemove: NSTableRowView, forRow: Int)

Tells the delegate that a row view was removed from the table at the specified row.

### Hiding and Showing Table Rows

func unhideRows(at: IndexSet, withAnimation: NSTableView.AnimationOptions)

Unhides the specified table rows.

var hiddenRowIndexes: IndexSet

The indexes of all hidden table rows.

