

- AppKit
- NSCollectionView
-  draggingImageForItems(at:with:offset:) 

Instance Method

# draggingImageForItems(at:with:offset:)

This method computes and returns an image to use for dragging.

macOS 10.6+

``` source
@MainActor
func draggingImageForItems(
    at indexes: IndexSet,
    with event: NSEvent,
    offset dragImageOffset: NSPointPointer
) -> NSImage
```

## Parameters 

`indexes`  

The index set of the items to be dragged.

`event`  

Mouse drag event.

`dragImageOffset`  

An in/out parameter that will initially be set to NSZeroPoint. it can be modified to reposition the returned image. A `dragImageOffset` of NSZeroPoint will cause the image to be centered under the mouse.

## Return Value

An image containing a rendering of the visible portions of the views for each item.

## Discussion

You can override the default image by subclassing NSCollectionView and overriding this method, or by implementing the collectionView(_:draggingImageForItemsAt:with:offset:) delegate method, it will be preferred over this method.

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

func frameForItem(at: Int) -> NSRect

Returns the frame of the collection view item at the specified index.

func frameForItem(at: Int, withNumberOfItems: Int) -> NSRect

Returns the frame of an item based on the number of items in the collection view.

func setDraggingSourceOperationMask(NSDragOperation, forLocal: Bool)

Configures the default value returned from draggingSourceOperationMaskForLocal:.

