

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:selectionIndexesForProposedSelection:) 

Instance Method

# outlineView(\_:selectionIndexesForProposedSelection:)

Invoked to allow the delegate to modify the proposed selection.

macOS 10.5+

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    selectionIndexesForProposedSelection proposedSelectionIndexes: IndexSet
) -> IndexSet
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`proposedSelectionIndexes`  

An index set containing the indexes of the proposed selection.

## Return Value

An NSIndexSet instance containing the indexes of the new selection. Return `proposedSelectionIndexes` if the proposed selection is acceptable, or the value of the table view’s existing selection to avoid changing the selection.

## Discussion

This method may be called multiple times with one new index added to the existing selection to find out if a particular index can be selected when the user is extending the selection with the keyboard or mouse.

Implementation of this method is optional. If implemented, this method will be called instead of outlineView(_:shouldSelectItem:).

## See Also

### Handling Selection

func outlineView(NSOutlineView, shouldSelect: NSTableColumn?) -> Bool

Returns a Boolean value that indicates whether the outline view should select a given table column.

func outlineView(NSOutlineView, shouldSelectItem: Any) -> Bool

Returns a Boolean value that indicates whether the outline view should select a given item.

func selectionShouldChange(in: NSOutlineView) -> Bool

Returns a Boolean value that indicates whether the outline view should change its selection.

func outlineViewSelectionIsChanging(Notification)

Invoked when `notification` is posted—that is, whenever the outline view’s selection changes.

func outlineViewSelectionDidChange(Notification)

Invoked when the selection did change notification is posted—that is, immediately after the outline view’s selection has changed.

