

- AppKit
- NSOutlineViewDelegate
-  selectionShouldChange(in:) 

Instance Method

# selectionShouldChange(in:)

Returns a Boolean value that indicates whether the outline view should change its selection.

macOS

``` source
@MainActor
optional func selectionShouldChange(in outlineView: NSOutlineView) -> Bool
```

## Parameters 

`outlineView`  

The outline view that sent the message.

## Return Value

true to permit `outlineView` to change its selection (typically a row being edited), false to deny permission.

## Discussion

For example, if the user is editing a cell and enters an improper value, the delegate can prevent the user from selecting or editing any other cells until a proper value has been entered into the original cell. The delegate can implement this method for complex validation of edited rows based on the values of any of their cells.

## See Also

### Handling Selection

func outlineView(NSOutlineView, shouldSelect: NSTableColumn?) -> Bool

Returns a Boolean value that indicates whether the outline view should select a given table column.

func outlineView(NSOutlineView, shouldSelectItem: Any) -> Bool

Returns a Boolean value that indicates whether the outline view should select a given item.

func outlineView(NSOutlineView, selectionIndexesForProposedSelection: IndexSet) -> IndexSet

Invoked to allow the delegate to modify the proposed selection.

func outlineViewSelectionIsChanging(Notification)

Invoked when `notification` is posted—that is, whenever the outline view’s selection changes.

func outlineViewSelectionDidChange(Notification)

Invoked when the selection did change notification is posted—that is, immediately after the outline view’s selection has changed.

