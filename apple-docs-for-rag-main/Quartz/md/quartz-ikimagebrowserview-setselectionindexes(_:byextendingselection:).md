

- Quartz
- IKImageBrowserView
-  setSelectionIndexes(\_:byExtendingSelection:) 

Instance Method

# setSelectionIndexes(\_:byExtendingSelection:)

Selects cells at the specified indexes.

macOS 10.4+

``` source
@MainActor
func setSelectionIndexes(
    _ indexes: IndexSet!,
    byExtendingSelection extendSelection: Bool
)
```

## Parameters 

`indexes`  

The indexes of the cells you want to select.

`extendSelection`  

A `BOOL` value that specifies whether to extend the current selection. Pass true to extends the selection; false replaces the current selection.

## See Also

### Reordering and Groups Items

func selectionIndexes() -> IndexSet!

Returns the indexes of the selected cells.

func setAllowsMultipleSelection(Bool)

Controls whether the user can select more than one cell at a time.

func allowsMultipleSelection() -> Bool

Returns whether multiple selections are allowed.

func setAllowsEmptySelection(Bool)

Controls whether an empty selection is allowed.

func allowsEmptySelection() -> Bool

Returns whether an empty selection is allowed.

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

