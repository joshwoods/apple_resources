

- AppKit
- NSOutlineViewDataSource
-  outlineView(\_:updateDraggingItemsForDrag:) 

Instance Method

# outlineView(\_:updateDraggingItemsForDrag:)

Implement this method to enable the table to update dragging items as they are dragged over the view.

macOS 10.7+

``` source
@MainActor
optional func outlineView(
    _ outlineView: NSOutlineView,
    updateDraggingItemsForDrag draggingInfo: any NSDraggingInfo
)
```

## Parameters 

`outlineView`  

The outline view in which the drag occurs.

`draggingInfo`  

The dragging info object.

## Discussion

Implementing this method is required for multi-image dragging. A typical implementation calls the passed-in dragging info object’s enumerateDraggingItems(options:for:classes:searchOptions:using:) method and sets the dragging item’s imageComponentsProvider property to a proper image based on the content. For NSView-based table views, you can use the `NSTableCellView` method draggingImageComponents.

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

func outlineView(NSOutlineView, validateDrop: any NSDraggingInfo, proposedItem: Any?, proposedChildIndex: Int) -> NSDragOperation

Used by an outline view to determine a valid drop target.

func outlineView(NSOutlineView, writeItems: [Any], to: NSPasteboard) -> Bool

Returns a Boolean value that indicates whether a drag operation is allowed.

Deprecated

