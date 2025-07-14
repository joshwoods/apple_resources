

- AppKit
- NSCollectionViewLayout
-  layoutAttributesForInterItemGap(before:) 

Instance Method

# layoutAttributesForInterItemGap(before:)

Returns layout attributes for the inter-item gap at the specified location in your layout.

macOS

``` source
@MainActor
func layoutAttributesForInterItemGap(before indexPath: IndexPath) -> NSCollectionViewLayoutAttributes?
```

## Parameters 

`indexPath`  

The index path of the item that follows the inter-item gap. For a gap that follows the last item in the section, set the item property to the total number of items in the section.

## Return Value

A layout attributes object containing the layout information to apply to the inter-item gap, or `nil` if no attributes are available.

## Discussion

The default implementation of this method returns `nil`. Subclasses can override this method to provide layout attributes for inter-item gaps. In your implementation, use the specified index path to compute the location of the gap in collection view’s content. If the gap represents a valid location, use the init(forInterItemGapBefore:) class method of NSCollectionViewLayoutAttributes to create a new layout attributes object and set the frame property to the rectangle you computed.

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

func layoutAttributesForDropTarget(at: NSPoint) -> NSCollectionViewLayoutAttributes?

Returns layout attributes for the drop target at the specified point.

func targetContentOffset(forProposedContentOffset: NSPoint) -> NSPoint

Returns the offset value to use after an animated layout update or change.

func targetContentOffset(forProposedContentOffset: NSPoint, withScrollingVelocity: NSPoint) -> NSPoint

Returns the offset value to use for the collection view’s content at the end of scrolling.

