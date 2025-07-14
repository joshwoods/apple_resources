

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:shouldSelectItem:) 

Instance Method

# outlineView(\_:shouldSelectItem:)

Returns a Boolean value that indicates whether the outline view should select a given item.

macOS

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    shouldSelectItem item: Any
) -> Bool
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`item`  

The item.

## Return Value

true to permit `outlineView` to select `item`, false to deny permission.

## Discussion

You implement this method to disallow selection of particular items.

For better performance and finer grain control over the selection, use outlineView(_:selectionIndexesForProposedSelection:).

## See Also

### Handling Selection

func outlineView(NSOutlineView, shouldSelect: NSTableColumn?) -> Bool

Returns a Boolean value that indicates whether the outline view should select a given table column.

func outlineView(NSOutlineView, selectionIndexesForProposedSelection: IndexSet) -> IndexSet

Invoked to allow the delegate to modify the proposed selection.

func selectionShouldChange(in: NSOutlineView) -> Bool

Returns a Boolean value that indicates whether the outline view should change its selection.

func outlineViewSelectionIsChanging(Notification)

Invoked when `notification` is posted—that is, whenever the outline view’s selection changes.

func outlineViewSelectionDidChange(Notification)

Invoked when the selection did change notification is posted—that is, immediately after the outline view’s selection has changed.

