

- AppKit
- NSCollectionView
-  newItem(forRepresentedObject:) Deprecated

Instance Method

# newItem(forRepresentedObject:)

Returns the collection view item that is used for the specified object.

macOS 10.5–10.14Deprecated

``` source
@MainActor
func newItem(forRepresentedObject object: Any) -> NSCollectionViewItem
```

Deprecated

Use -\[NSCollectionViewDataSource collectionView:itemForRepresentedObjectAtIndexPath:\] instead

## Parameters 

`object`  

The content object that the collection view item will represent.

## Return Value

An initialized collection view item with the specified object and the appropriate view set. The collection view item should not be autoreleased.

## Discussion

Whenever possible, register classes or nib files for your items instead of using this property. For more information, see Creating Collection View Items.

Subclasses can override this method if the collection view items are not generated from a prototype or if the prototype view needs to be modified. The subclass is responsible for setting the `view` and representedObject of the new collection view item.

## See Also

### Legacy Collection View Support

var itemPrototype: NSCollectionViewItem?

The receiver’s collection view item prototype.

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

func draggingImageForItems(at: IndexSet, with: NSEvent, offset: NSPointPointer) -> NSImage

This method computes and returns an image to use for dragging.

func setDraggingSourceOperationMask(NSDragOperation, forLocal: Bool)

Configures the default value returned from draggingSourceOperationMaskForLocal:.

