

- AppKit
- NSOutlineViewDataSource
-  outlineView(\_:acceptDrop:item:childIndex:) 

Instance Method

# outlineView(\_:acceptDrop:item:childIndex:)

Returns a Boolean value that indicates whether a drop operation was successful.

macOS

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    acceptDrop info: any NSDraggingInfo,
    item: Any?,
    childIndex index: Int
) -> Bool
```

## Parameters 

`outlineView`  

The outline view that sent the message. `outlineView` must have previously allowed a drop.

`info`  

An object that contains more information about this dragging operation.

`item`  

The parent of the item over which the cursor was placed when the mouse button was released.

`index`  

The index of the child of `item` over which the cursor was placed when the mouse button was released.

## Return Value

true if the drop operation was successful, otherwise false.

## Discussion

The data source should incorporate the data from the dragging pasteboard in the implementation of this method. You can get the data for the drop operation from info using the draggingPasteboard method.

The return value indicates success or failure of the drag operation to the system.

## See Also

### Related Documentation

func shouldCollapseAutoExpandedItems(forDeposited: Bool) -> Bool

Returns a Boolean value that indicates whether auto-expanded items should return to their original collapsed state.

### Instance Methods

func outlineView(NSOutlineView, child: Int, ofItem: Any?) -> Any

Returns the child item at the specified index of a given item.

func outlineView(NSOutlineView, draggingSession: NSDraggingSession, endedAt: NSPoint, operation: NSDragOperation)

Implement this method to know when the given dragging session has ended.

func outlineView(NSOutlineView, draggingSession: NSDraggingSession, willBeginAt: NSPoint, forItems: [Any])

Implement this method know when the given dragging session is about to begin and potentially modify the dragging session.

func outlineView(NSOutlineView, isItemExpandable: Any) -> Bool

Returns a Boolean value that indicates whether the a given item is expandable.

func outlineView(NSOutlineView, itemForPersistentObject: Any) -> Any?

Invoked by `outlineView` to return the item for the archived `object`.

func outlineView(NSOutlineView, namesOfPromisedFilesDroppedAtDestination: URL, forDraggedItems: [Any]) -> [String]

Returns an array of filenames for the created files that the receiver promises to create.

Deprecated

func outlineView(NSOutlineView, numberOfChildrenOfItem: Any?) -> Int

Returns the number of child items encompassed by a given item.

func outlineView(NSOutlineView, objectValueFor: NSTableColumn?, byItem: Any?) -> Any?

Invoked by `outlineView` to return the data object associated with the specified `item`.

func outlineView(NSOutlineView, pasteboardWriterForItem: Any) -> (any NSPasteboardWriting)?

Implement this method to enable the table to be an `NSDraggingSource` that supports dragging multiple items.

func outlineView(NSOutlineView, persistentObjectForItem: Any?) -> Any?

Invoked by `outlineView` to return an archived object for `item`.

func outlineView(NSOutlineView, setObjectValue: Any?, for: NSTableColumn?, byItem: Any?)

Set the data object for a given item in a given column.

func outlineView(NSOutlineView, sortDescriptorsDidChange: [NSSortDescriptor])

Invoked by an outline view to notify the data source that the descriptors changed and the data may need to be resorted.

func outlineView(NSOutlineView, updateDraggingItemsForDrag: any NSDraggingInfo)

Implement this method to enable the table to update dragging items as they are dragged over the view.

func outlineView(NSOutlineView, validateDrop: any NSDraggingInfo, proposedItem: Any?, proposedChildIndex: Int) -> NSDragOperation

Used by an outline view to determine a valid drop target.

func outlineView(NSOutlineView, writeItems: [Any], to: NSPasteboard) -> Bool

Returns a Boolean value that indicates whether a drag operation is allowed.

Deprecated

