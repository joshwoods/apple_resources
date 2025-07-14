

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:validateDrop:proposedIndex:dropOperation:) 

Instance Method

# collectionView(\_:validateDrop:proposedIndex:dropOperation:)

Validates the specified location to see if it is a valid drop target.

macOS 10.6+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    validateDrop draggingInfo: any NSDraggingInfo,
    proposedIndex proposedDropIndex: UnsafeMutablePointer,
    dropOperation proposedDropOperation: UnsafeMutablePointer
) -> NSDragOperation
```

## Parameters 

`collectionView`  

The collection view that send the message.

`draggingInfo`  

An object containing details about this dragging operation.

`proposedDropIndex`  

The proposed drop index. This parameter is passed by-reference and can be modified retarget the drop operation.

`proposedDropOperation`  

The proposed drop operation. This parameter is passed by-reference and can be modified to change the drop operation.

## Return Value

A value that indicates which dragging operation to perform. Return NSDragOperationNone to disallow the drop.

## Discussion

Based on the mouse position, the collection view will suggest a proposed index and drop operation. These values are in/out parameters and can be changed by the delegate to retarget the drop operation.

The collection view will propose `NSCollectionViewDropOn` when the dragging location is closer to the middle of the item than either of its edges. Otherwise, it will propose `NSCollectionViewDropBefore`. You may override this default behavior by changing `proposedDropOperation` or `proposedDropIndex`.

To receive drag messages, you must first send registerForDraggedTypes(_:) to the collection view with the drag types you want to support.

You must implement this method for your collection view to be a drag destination.

## See Also

### Legacy Collection View Support

func collectionView(NSCollectionView, canDragItemsAt: IndexSet, with: NSEvent) -> Bool

Returns a Boolean indicating whether the collection view can begin dragging the specified items.

func collectionView(NSCollectionView, pasteboardWriterForItemAt: Int) -> (any NSPasteboardWriting)?

Provides the pasteboard writer for the item at the specified index

func collectionView(NSCollectionView, writeItemsAt: IndexSet, to: NSPasteboard) -> Bool

Invoked after it has been determined that a drag should begin, but before the drag has been started.

Deprecated

func collectionView(NSCollectionView, namesOfPromisedFilesDroppedAtDestination: URL, forDraggedItemsAt: IndexSet) -> [String]

Invoked to return an array of filenames that the receiver promises to create.

Deprecated

func collectionView(NSCollectionView, draggingImageForItemsAt: IndexSet, with: NSEvent, offset: NSPointPointer) -> NSImage

Creates and returns a drag image to represent the specified items during a drag.

func collectionView(NSCollectionView, draggingSession: NSDraggingSession, willBeginAt: NSPoint, forItemsAt: IndexSet)

Notifies your delegate that a drag session is about to begin.

func collectionView(NSCollectionView, acceptDrop: any NSDraggingInfo, index: Int, dropOperation: NSCollectionView.DropOperation) -> Bool

Invoked when the mouse is released over a collection view that previously allowed a drop.

