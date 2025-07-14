

- AppKit
-  NSOutlineViewDataSource 

Protocol

# NSOutlineViewDataSource

A set of methods that an outline view calls to retrieve data and information about it from the data source delegate, and—optionally—to update data values.

macOS

``` source
protocol NSOutlineViewDataSource : NSObjectProtocol
```

## Overview

NSOutlineView objects support a data source delegate in addition to the regular delegate object.

All the methods in the NSOutlineViewDataSource protocol are marked as `@optional`. While this is true, there are cases were you must implement some methods to achieve required functionality, specifically when working with conventional data sources rather than data that is provided by Cocoa bindings.

### Required and Optional Methods Using Programmatic Conventions and Cocoa Bindings

If you are using conventional data sources for content you must implement the basic methods that provide the outline view with data: outlineView(_:child:ofItem:), outlineView(_:isItemExpandable:), outlineView(_:numberOfChildrenOfItem:), and outlineView(_:objectValueFor:byItem:). Applications that acquire their data using Cocoa bindings do not need to implement these methods.

Similarly, when using conventional data sources , if you want to allow the user to edit values, you must implement outlineView(_:setObjectValue:for:byItem:). When these methods are invoked by the outline view, `nil` as the `item` refers to the “root” item. `NSOutlineView` requires that each item in the outline view be unique. In order for the collapsed state of an outline view to remain consistent between reloads you must always return the same object for an item. When using Cocoa bindings to provide outline view content, there is no requirement to implement this method.

Note

Some of the methods in this `protocol`, such as outlineView(_:child:ofItem:) and outlineView(_:numberOfChildrenOfItem:) along with other methods that return data, are called very frequently, so they must be efficient.

## Topics

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

func outlineView(NSOutlineView, validateDrop: any NSDraggingInfo, proposedItem: Any?, proposedChildIndex: Int) -> NSDragOperation

Used by an outline view to determine a valid drop target.

func outlineView(NSOutlineView, writeItems: [Any], to: NSPasteboard) -> Bool

Returns a Boolean value that indicates whether a drag operation is allowed.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Management

protocol NSOutlineViewDelegate

A set of optional methods implemented by delegates of NSOutlineView objects.

