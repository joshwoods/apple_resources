

- Quartz
- IKImageBrowserView
-  allowsEmptySelection() 

Instance Method

# allowsEmptySelection()

Returns whether an empty selection is allowed.

macOS 10.4+

``` source
@MainActor
func allowsEmptySelection() -> Bool
```

## Return Value

true if the receiver allows an empty selection; false otherwise.

## See Also

### Reordering and Groups Items

func selectionIndexes() -> IndexSet!

Returns the indexes of the selected cells.

func setSelectionIndexes(IndexSet!, byExtendingSelection: Bool)

Selects cells at the specified indexes.

func setAllowsMultipleSelection(Bool)

Controls whether the user can select more than one cell at a time.

func allowsMultipleSelection() -> Bool

Returns whether multiple selections are allowed.

func setAllowsEmptySelection(Bool)

Controls whether an empty selection is allowed.

func setAllowsReordering(Bool)

Controls whether the user can reorder items.

func allowsReordering() -> Bool

Returns whether the user can reorder items.

func setAnimates(Bool)

Controls whether the receiver animates reordering and changes of the data source.

func animates() -> Bool

Returns whether the receiver animates reordering and changes of the data source.

func expandGroup(at: Int)

Expands a group at the specified index.

func collapseGroup(at: Int)

Collapses a group at the specified index.

func isGroupExpanded(at: Int) -> Bool

Returns whether the group at the provided index is expanded.

