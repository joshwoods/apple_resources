

- AppKit
- NSOutlineViewDataSource
-  outlineView(\_:namesOfPromisedFilesDroppedAtDestination:forDraggedItems:) Deprecated

Instance Method

# outlineView(\_:namesOfPromisedFilesDroppedAtDestination:forDraggedItems:)

Returns an array of filenames for the created files that the receiver promises to create.

macOS 10.0–10.13Deprecated

``` source
optional func outlineView(
    _ outlineView: NSOutlineView,
    namesOfPromisedFilesDroppedAtDestination dropDestination: URL,
    forDraggedItems items: [Any]
) -> [String]
```

Deprecated

Use NSFilePromiseReceiver objects instead

## Parameters 

`outlineView`  

The outline view that sent the message.

`dropDestination`  

The drop location where the files are created.

`items`  

The items being dragged.

## Return Value

An array of filenames (not full paths) for the created files that the receiver promises to create.

## Discussion

For more information on file promise dragging, see documentation on the `NSDraggingSource` protocol and namesOfPromisedFilesDropped(atDestination:).

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

