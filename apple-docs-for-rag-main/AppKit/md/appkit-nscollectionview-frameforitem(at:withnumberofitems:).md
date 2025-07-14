

- AppKit
- NSCollectionView
-  frameForItem(at:withNumberOfItems:) 

Instance Method

# frameForItem(at:withNumberOfItems:)

Returns the frame of an item based on the number of items in the collection view.

macOS 10.7+

``` source
@MainActor
func frameForItem(
    at index: Int,
    withNumberOfItems numberOfItems: Int
) -> NSRect
```

## Parameters 

`index`  

The index of the item in the collection view.

`numberOfItems`  

The targeted number of items in the collection view. Use this parameter to specify the number of items you intend to have in the collection view, if that number is different than the actual number of items.

## Return Value

The frame rectangle that reflects where the collection view would place the item.

## Discussion

Using the value in the `numberOfItems` parameter, this method calculates the frame rectangle of the item at the specified `index` in the collection view.

When the collection view is a drag destination, use this method (instead of the content method) to get the frame of items. Drag operations can change the number of items, which affects the layout of the item views.

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

func draggingImageForItems(at: IndexSet, with: NSEvent, offset: NSPointPointer) -> NSImage

This method computes and returns an image to use for dragging.

func setDraggingSourceOperationMask(NSDragOperation, forLocal: Bool)

Configures the default value returned from draggingSourceOperationMaskForLocal:.

