

- AppKit
- NSCollectionViewLayout
-  layoutAttributesClass 

Type Property

# layoutAttributesClass

Returns the class to use for layout attribute objects

macOS

``` source
@MainActor
class var layoutAttributesClass: AnyClass { get }
```

## Return Value

The class to use for layout attribute objects.

## Discussion

Override this method if you define a custom NSCollectionViewLayoutAttributes subclass for managing layout-related attributes. In your implementation, return the class object for your custom subclass.

You can call this method as needed to create new layout objects. A typical usage of this method is as follows:

- Swift
- Objective-C

```
let attributes = MyCustomLayout.layoutAttributesClass().init()
```

```
id attributes = [[[MyCustomLayout layoutAttributesClass] alloc] init];
```

## See Also

### Providing Layout Information

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

func layoutAttributesForInterItemGap(before: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns layout attributes for the inter-item gap at the specified location in your layout.

func targetContentOffset(forProposedContentOffset: NSPoint) -> NSPoint

Returns the offset value to use after an animated layout update or change.

func targetContentOffset(forProposedContentOffset: NSPoint, withScrollingVelocity: NSPoint) -> NSPoint

Returns the offset value to use for the collection view’s content at the end of scrolling.

