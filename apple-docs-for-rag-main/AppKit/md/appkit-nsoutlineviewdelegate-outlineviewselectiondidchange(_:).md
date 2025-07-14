

- AppKit
- NSOutlineViewDelegate
-  outlineViewSelectionDidChange(\_:) 

Instance Method

# outlineViewSelectionDidChange(\_:)

Invoked when the selection did change notification is posted—that is, immediately after the outline view’s selection has changed.

macOS 10.10+

``` source
@MainActor
optional func outlineViewSelectionDidChange(_ notification: Notification)
```

## Parameters 

`notification`  

The posted notification.

## Discussion

This method is invoked as a result of posting an selectionDidChangeNotification.

## See Also

### Handling Selection

func outlineView(NSOutlineView, shouldSelect: NSTableColumn?) -> Bool

Returns a Boolean value that indicates whether the outline view should select a given table column.

func outlineView(NSOutlineView, shouldSelectItem: Any) -> Bool

Returns a Boolean value that indicates whether the outline view should select a given item.

func outlineView(NSOutlineView, selectionIndexesForProposedSelection: IndexSet) -> IndexSet

Invoked to allow the delegate to modify the proposed selection.

func selectionShouldChange(in: NSOutlineView) -> Bool

Returns a Boolean value that indicates whether the outline view should change its selection.

func outlineViewSelectionIsChanging(Notification)

Invoked when `notification` is posted—that is, whenever the outline view’s selection changes.

