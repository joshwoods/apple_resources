

- AppKit
- NSTableView
-  hiddenRowIndexes 

Instance Property

# hiddenRowIndexes

The indexes of all hidden table rows.

macOS 10.11+

``` source
@MainActor
var hiddenRowIndexes: IndexSet { get }
```

## Discussion

The value of this property is an index set containing the indexes of any hidden table rows. Table rows may be hidden by invoking the hideRows(at:withAnimation:) method. Some drag-and-drop operations also result in hidden rows.

## See Also

### Hiding and Showing Table Rows

func hideRows(at: IndexSet, withAnimation: NSTableView.AnimationOptions)

Hides the specified table rows.

func unhideRows(at: IndexSet, withAnimation: NSTableView.AnimationOptions)

Unhides the specified table rows.

