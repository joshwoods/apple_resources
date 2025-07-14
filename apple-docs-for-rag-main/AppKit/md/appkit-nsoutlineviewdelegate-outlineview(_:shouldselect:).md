

- AppKit
- NSOutlineViewDelegate
-  outlineView(\_:shouldSelect:) 

Instance Method

# outlineView(\_:shouldSelect:)

Returns a Boolean value that indicates whether the outline view should select a given table column.

macOS

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    shouldSelect tableColumn: NSTableColumn?
) -> Bool
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`tableColumn`  

The table column.

## Return Value

true to permit `outlineView` to select `tableColumn`, false to deny permission.

## Discussion

The delegate can implement this method to disallow selection of specific columns.

## See Also

### Handling Selection

func outlineView(NSOutlineView, shouldSelectItem: Any) -> Bool

Returns a Boolean value that indicates whether the outline view should select a given item.

func outlineView(NSOutlineView, selectionIndexesForProposedSelection: IndexSet) -> IndexSet

Invoked to allow the delegate to modify the proposed selection.

func selectionShouldChange(in: NSOutlineView) -> Bool

Returns a Boolean value that indicates whether the outline view should change its selection.

func outlineViewSelectionIsChanging(Notification)

Invoked when `notification` is posted—that is, whenever the outline view’s selection changes.

func outlineViewSelectionDidChange(Notification)

Invoked when the selection did change notification is posted—that is, immediately after the outline view’s selection has changed.

