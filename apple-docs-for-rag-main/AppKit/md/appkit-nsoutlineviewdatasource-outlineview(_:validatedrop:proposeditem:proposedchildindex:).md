

- AppKit
- NSOutlineViewDataSource
-  outlineView(\_:validateDrop:proposedItem:proposedChildIndex:) 

Instance Method

# outlineView(\_:validateDrop:proposedItem:proposedChildIndex:)

Used by an outline view to determine a valid drop target.

macOS

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    validateDrop info: any NSDraggingInfo,
    proposedItem item: Any?,
    proposedChildIndex index: Int
) -> NSDragOperation
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`info`  

An object that contains more information about this dragging operation.

`item`  

The proposed parent.

`index`  

The proposed child location.

## Return Value

A value that indicates which dragging operation the data source will perform.

## Discussion

Based on the mouse position, the outline view will suggest a proposed drop location. The data source may “retarget” a drop if desired by calling setDropItem(_:dropChildIndex:) and returning something other than `NSDragOperationNone`. You may choose to retarget for various reasons (for example, for better visual feedback when inserting into a sorted position).

Implementation of this method is optional.

## See Also

### Instance Methods

func outlineView(NSOutlineView, acceptDrop: any NSDraggingInfo, item: Any?, childIndex: Int) -> Bool

Returns a Boolean value that indicates whether a drop operation was successful.

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

func outlineView(NSOutlineView, writeItems: [Any], to: NSPasteboard) -> Bool

Returns a Boolean value that indicates whether a drag operation is allowed.

Deprecated

