

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:validateDrop:proposedIndexPath:dropOperation:) 

Instance Method

# collectionView(\_:validateDrop:proposedIndexPath:dropOperation:)

Validates whether a drop operation is possible at the specified location.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    validateDrop draggingInfo: any NSDraggingInfo,
    proposedIndexPath proposedDropIndexPath: AutoreleasingUnsafeMutablePointer,
    dropOperation proposedDropOperation: UnsafeMutablePointer
) -> NSDragOperation
```

## Parameters 

`collectionView`  

The collection view asking you to validate the drop operation.

`draggingInfo`  

The information about the drag operation.

`proposedDropIndexPath`  

The index path at which the drop would occur. This parameter is passed by-reference and can be modified to change the proposed index path.

`proposedDropOperation`  

The type of drop operation being proposed. This parameter is passed by-reference and can be modified to change the drop operation type.

## Return Value

A value that indicates which dragging operation to perform. Return NSDragOperationNone to disallow a drop at the proposed location.

## Discussion

Although implementation of this method is optional, you must implement it to support drops onto the associated collection view. You must also call the collection view’s registerForDraggedTypes(_:) method to register the types of drops it supports. If you do not perform both of these actions, the collection view does not accept drops.

When an interactive drag operation occurs, the collection view calls this method to determine whether the current mouse location is a valid place to drop the content. This method may be called many times during the course of the drag operation. Your implementation should look at the proposed location and return a constant that reflects how the drop would be handled.

While validating the drop location, you can suggest a better drop location by updating the values in the `proposedDropIndexPath` and `proposedDropOperation` parameters. For example, you might suggest dropping the content before the specified item instead of on it. The collection view sets the `proposedDropOperation` parameter to NSCollectionView.DropOperation.on when the mouse is closer to the middle of an item than to its edges; otherwise, it sets the parameter to NSCollectionView.DropOperation.before.

## See Also

### Drag and Drop Support

Supporting Collection View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

func collectionView(NSCollectionView, canDragItemsAt: Set&lt;IndexPath>, with: NSEvent) -> Bool

Returns a Boolean indicating whether a drag operation involving the specified items can begin.

func collectionView(NSCollectionView, pasteboardWriterForItemAt: IndexPath) -> (any NSPasteboardWriting)?

Provides the pasteboard writer for the item at the specified index path.

func collectionView(NSCollectionView, writeItemsAt: Set&lt;IndexPath>, to: NSPasteboard) -> Bool

Places the data for the drag operation on the pasteboard.

Deprecated

func collectionView(NSCollectionView, namesOfPromisedFilesDroppedAtDestination: URL, forDraggedItemsAt: Set&lt;IndexPath>) -> [String]

Returns the names of the promised files that you created for a drag operation.

Deprecated

func collectionView(NSCollectionView, draggingImageForItemsAt: Set&lt;IndexPath>, with: NSEvent, offset: NSPointPointer) -> NSImage

Creates and returns a drag image to represent the specified items during a drag.

func collectionView(NSCollectionView, draggingSession: NSDraggingSession, willBeginAt: NSPoint, forItemsAt: Set&lt;IndexPath>)

Notifies your delegate that a drag session is about to begin.

func collectionView(NSCollectionView, draggingSession: NSDraggingSession, endedAt: NSPoint, dragOperation: NSDragOperation)

Notifies your delegate that a drag session ended.

func collectionView(NSCollectionView, updateDraggingItemsForDrag: any NSDraggingInfo)

Asks your delegate to update the dragging items during a drag operation.

func collectionView(NSCollectionView, acceptDrop: any NSDraggingInfo, indexPath: IndexPath, dropOperation: NSCollectionView.DropOperation) -> Bool

Incorporates the dropped content into the collection view.

