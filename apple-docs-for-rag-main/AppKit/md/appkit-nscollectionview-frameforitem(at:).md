

- AppKit
- NSCollectionView
-  frameForItem(at:) 

Instance Method

# frameForItem(at:)

Returns the frame of the collection view item at the specified index.

macOS 10.6+

``` source
@MainActor
func frameForItem(at index: Int) -> NSRect
```

## Parameters 

`index`  

The index of the collection view item.

## Return Value

The frame calculated by the receiver where it intends to place the subview for the NSCollectionViewItem at the given index. The rectangle is returned in the collection view’s coordinate system.

## Discussion

You can use this method in the collectionView(_:draggingImageForItemsAt:with:offset:) method to determine which views are in the visible portion of the enclosing scroll view.

Overriding this method will have no effect on the collection view’s subview layout.

## See Also

### Legacy Collection View Support

var itemPrototype: NSCollectionViewItem?

The receiver’s collection view item prototype.

Deprecated

func newItem(forRepresentedObject: Any) -> NSCollectionViewItem

Returns the collection view item that is used for the specified object.

Deprecated

var selectionIndexes: IndexSet

The indexes of the currently selected items.

var maxNumberOfRows: Int

The maximum number of rows that the collection view displays.

Deprecated

var maxNumberOfColumns: Int

The maximum number of columns that the collection view displays.

Deprecated

var minItemSize: NSSize

The minimum size (in points) of items in the collection view grid.

Deprecated

var maxItemSize: NSSize

The maximum size (in points) of items in the collection view grid.

Deprecated

func item(at: Int) -> NSCollectionViewItem?

Returns the collection view item for the represented object at the specified index.

func frameForItem(at: Int, withNumberOfItems: Int) -> NSRect

Returns the frame of an item based on the number of items in the collection view.

func draggingImageForItems(at: IndexSet, with: NSEvent, offset: NSPointPointer) -> NSImage

This method computes and returns an image to use for dragging.

func setDraggingSourceOperationMask(NSDragOperation, forLocal: Bool)

Configures the default value returned from draggingSourceOperationMaskForLocal:.

