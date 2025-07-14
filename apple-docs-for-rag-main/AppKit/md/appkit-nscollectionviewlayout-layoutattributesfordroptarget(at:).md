

- AppKit
- NSCollectionViewLayout
-  layoutAttributesForDropTarget(at:) 

Instance Method

# layoutAttributesForDropTarget(at:)

Returns layout attributes for the drop target at the specified point.

macOS

``` source
@MainActor
func layoutAttributesForDropTarget(at pointInCollectionView: NSPoint) -> NSCollectionViewLayoutAttributes?
```

## Parameters 

`pointInCollectionView`  

A point in the collection view’s coordinate system. Use this point to determine whether the drop would occur on an item or between items.

## Return Value

A layout attributes object that identifies the element in which the drop would occur.

## Discussion

The default implementation of this method tests the specified point to see if it lands inside an item, supplementary view, or decoration view of the collection view. If it does, the method returns the layout attributes for that element.

Layouts that support inter-item gaps as drop targets must override this method and use it to return the layout attributes that represent that gap. In your implementation, calculate the index path just after the gap and pass that value to the init(forInterItemGapBefore:) class method of NSCollectionViewLayoutAttributes. Set the frame property of the resulting attributes object to the rectangle that best represents the gap and also contains the specified point. When overriding this method, you can call `super` at any time to get the default behavior.

## See Also

### Providing Layout Information

class var layoutAttributesClass: AnyClass

Returns the class to use for layout attribute objects

func prepare()

Prepares the layout object to begin laying out content.

var collectionViewContentSize: NSSize

The width and height of the collection view’s contents.

func layoutAttributesForElements(in: NSRect) -> [NSCollectionViewLayoutAttributes]

Returns the layout attribute objects for all items and views in the specified rectangle.

func layoutAttributesForItem(at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the layout attributes for the item at the specified index path.

func layoutAttributesForSupplementaryView(ofKind: NSCollectionView.SupplementaryElementKind, at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the layout attributes of the supplementary view at the specified location in your layout.

func layoutAttributesForDecorationView(ofKind: NSCollectionView.DecorationElementKind, at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the layout attributes of the decoration view at the specified location in your layout.

func layoutAttributesForInterItemGap(before: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns layout attributes for the inter-item gap at the specified location in your layout.

func targetContentOffset(forProposedContentOffset: NSPoint) -> NSPoint

Returns the offset value to use after an animated layout update or change.

func targetContentOffset(forProposedContentOffset: NSPoint, withScrollingVelocity: NSPoint) -> NSPoint

Returns the offset value to use for the collection view’s content at the end of scrolling.

