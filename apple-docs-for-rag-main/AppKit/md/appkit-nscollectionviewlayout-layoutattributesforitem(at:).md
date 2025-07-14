

- AppKit
- NSCollectionViewLayout
-  layoutAttributesForItem(at:) 

Instance Method

# layoutAttributesForItem(at:)

Returns the layout attributes for the item at the specified index path.

macOS

``` source
@MainActor
func layoutAttributesForItem(at indexPath: IndexPath) -> NSCollectionViewLayoutAttributes?
```

## Parameters 

`indexPath`  

The index path of the item whose attributes are requested.

## Return Value

A layout attributes object containing the layout information to apply to the item.

## Discussion

Subclasses must override this method. In your implementation, create an instance of the appropriate layout attributes class and fill the resulting object with the layout information for the specified item. The default implementation of this method does nothing and returns `nil`.

You can also call this method from other layout-related methods when you want to retrieve layout information for items. Call this method only for items. Do not call it to retrieve layout attributes for supplementary views or decoration views.

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

func layoutAttributesForSupplementaryView(ofKind: NSCollectionView.SupplementaryElementKind, at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the layout attributes of the supplementary view at the specified location in your layout.

func layoutAttributesForDecorationView(ofKind: NSCollectionView.DecorationElementKind, at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the layout attributes of the decoration view at the specified location in your layout.

func layoutAttributesForDropTarget(at: NSPoint) -> NSCollectionViewLayoutAttributes?

Returns layout attributes for the drop target at the specified point.

func layoutAttributesForInterItemGap(before: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns layout attributes for the inter-item gap at the specified location in your layout.

func targetContentOffset(forProposedContentOffset: NSPoint) -> NSPoint

Returns the offset value to use after an animated layout update or change.

func targetContentOffset(forProposedContentOffset: NSPoint, withScrollingVelocity: NSPoint) -> NSPoint

Returns the offset value to use for the collection view’s content at the end of scrolling.

