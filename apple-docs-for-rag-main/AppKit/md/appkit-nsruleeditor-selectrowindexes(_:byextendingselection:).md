

- AppKit
- NSRuleEditor
-  selectRowIndexes(\_:byExtendingSelection:) 

Instance Method

# selectRowIndexes(\_:byExtendingSelection:)

Sets in the receiver the indexes of rows that are selected.

macOS

``` source
@MainActor
func selectRowIndexes(
    _ indexes: IndexSet,
    byExtendingSelection extend: Bool
)
```

## Parameters 

`indexes`  

The indexes of rows in the receiver to select.

Important

Raises an `NSRangeException` if any index in `rowIndexes` is less than `0` or greater than or equal to the number of rows.

`extend`  

If false, the selected rows are specified by `indexes`. If true, the rows indicated by `indexes` are added to the collection of already selected rows, providing multiple selection.

## See Also

### Working with the Selection

var selectedRowIndexes: IndexSet

The indexes of the rule editor’s selected rows.

