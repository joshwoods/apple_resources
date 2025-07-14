

- AppKit
- NSOutlineViewDataSource
-  outlineView(\_:child:ofItem:) 

Instance Method

# outlineView(\_:child:ofItem:)

Returns the child item at the specified index of a given item.

macOS

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    child index: Int,
    ofItem item: Any?
) -> Any
```

## Parameters 

`outlineView`  

The outline view that sent the message.

`index`  

The index of the child item from `item` to return.

`item`  

An item in the data source.

## Return Value

The child item at `index` of `item`. If `item` is `nil`, returns the appropriate child item of the root object.

## Discussion

Children of a given parent `item` are accessed sequentially. In order for the collapsed state of the outline view to remain consistent when it is reloaded you must always return the same object for a specified `child` and `item`.

Important

While this method is marked as `@optional` in the protocol, **you must implement this method if you are not providing the data for the outline view using Cocoa bindings.**

Do not call reloadData() from this method.

### Special Considerations

The outlineView(_:child:ofItem:) method is called very frequently, so it must be efficient.

## See Also

### Related Documentation

func outlineView(NSOutlineView, numberOfChildrenOfItem: Any?) -> Int

Returns the number of child items encompassed by a given item.

Outline View Programming Topics

### Instance Methods

func outlineView(NSOutlineView, acceptDrop: any NSDraggingInfo, item: Any?, childIndex: Int) -> Bool

Returns a Boolean value that indicates whether a drop operation was successful.

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

