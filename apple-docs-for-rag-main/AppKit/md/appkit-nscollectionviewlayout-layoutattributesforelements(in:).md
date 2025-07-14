

- AppKit
- NSCollectionViewLayout
-  layoutAttributesForElements(in:) 

Instance Method

# layoutAttributesForElements(in:)

Returns the layout attribute objects for all items and views in the specified rectangle.

macOS

``` source
@MainActor
func layoutAttributesForElements(in rect: NSRect) -> [NSCollectionViewLayoutAttributes]
```

## Parameters 

`rect`  

The rectangle (specified in the collection view’s coordinate system) containing the target views.

## Return Value

An array of layout attribute objects containing the layout information for the enclosed items and views.

## Discussion

Subclasses must override this method. In your implementation, return layout attributes for all items, supplementary views, and decoration views that intersect the specified rectangle.

For each element, always return a layout object of the appropriate type (item, supplementary, or decoration). The collection view differentiates between attributes for items, supplementary views, and decoration views and uses the differences to decide how to create and manage the corresponding views. Use the layoutAttributesForItem(at:), layoutAttributesForSupplementaryView(ofKind:at:), and layoutAttributesForDecorationView(ofKind:at:) methods to create new layout attribute objects.

## See Also

### Providing Layout Information

class var layoutAttributesClass: AnyClass

Returns the class to use for layout attribute objects

func prepare()

Prepares the layout object to begin laying out content.

var collectionViewContentSize: NSSize

The width and height of the collection view’s contents.

func layoutAttributesForItem(at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the layout attributes for the item at the specified index path.

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

