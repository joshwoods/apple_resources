

- Quartz
- IKImageBrowserView
-  isGroupExpanded(at:) 

Instance Method

# isGroupExpanded(at:)

Returns whether the group at the provided index is expanded.

macOS 10.4+

``` source
@MainActor
func isGroupExpanded(at index: Int) -> Bool
```

## Parameters 

`index`  

The index you want to check.

## Return Value

true if the group is expanded; false otherwise.

## Discussion

This method is declared in OS X v10.5, but an implementation was not provided until OS X v10.6. Avoid using this method in OS X v10.5.

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

