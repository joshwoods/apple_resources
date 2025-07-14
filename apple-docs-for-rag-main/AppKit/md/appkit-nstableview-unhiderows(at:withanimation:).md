

- AppKit
- NSTableView
-  unhideRows(at:withAnimation:) 

Instance Method

# unhideRows(at:withAnimation:)

Unhides the specified table rows.

macOS 10.11+

``` source
@MainActor
func unhideRows(
    at indexes: IndexSet,
    withAnimation rowAnimation: NSTableView.AnimationOptions = []
)
```

## Parameters 

`indexes`  

An index set containing indexes of the hidden rows to be shown again.

`rowAnimation`  

An animation effect to be applied when the rows are hidden.

## Discussion

Unhiding a table row causes the tableView(_:didAdd:forRow:) delegate method to be invoked.

## See Also

### Related Documentation

struct AnimationOptions

Specifies the animation effects to apply when inserting or removing rows.

func tableView(NSTableView, didAdd: NSTableRowView, forRow: Int)

Tells the delegate that a row view was added at the specified row.

### Hiding and Showing Table Rows

func hideRows(at: IndexSet, withAnimation: NSTableView.AnimationOptions)

Hides the specified table rows.

var hiddenRowIndexes: IndexSet

The indexes of all hidden table rows.

