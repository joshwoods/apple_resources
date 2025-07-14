

- UIKit
- UICollectionViewLayout
-  layoutAttributesForInteractivelyMovingItem(at:withTargetPosition:) 

Instance Method

# layoutAttributesForInteractivelyMovingItem(at:withTargetPosition:)

Retrieves the layout attributes of an item when it is being moved interactively by the user.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func layoutAttributesForInteractivelyMovingItem(
    at indexPath: IndexPath,
    withTargetPosition position: CGPoint
) -> UICollectionViewLayoutAttributes
```

## Parameters 

`indexPath`  

The index path of the item being moved.

`position`  

The current position of the item in the collection view’s coordinate system.

## Return Value

The layout attributes of the item while it is at the specified position.

## Discussion

When an item is moving because of user interactivity, the layout object uses this method to retrieve layout attributes to use for the item while it is at the specified position. The default implementation of this method returns a copy of the item’s existing attributes with two changes: the center point is set to the value in `position` and the zIndex value is set to NSIntegerMax so that the item floats above other items in the collection view.

Subclasses can override this method and modify additional layout attributes as needed. If you override this method, call `super` first to retrieve the item’s existing attributes and then make your changes to the returned structure.

## See Also

### Providing layout attributes

class var layoutAttributesClass: AnyClass

The class to use when creating layout attributes objects.

func prepare()

Tells the layout object to update the current layout.

func layoutAttributesForElements(in: CGRect) -> [UICollectionViewLayoutAttributes]?

Retrieves the layout attributes for all of the cells and views in the specified rectangle.

func layoutAttributesForItem(at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves layout information for an item at the specified index path with a corresponding cell.

func layoutAttributesForSupplementaryView(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves the layout attributes for the specified supplementary view.

func layoutAttributesForDecorationView(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves the layout attributes for the specified decoration view.

func targetContentOffset(forProposedContentOffset: CGPoint) -> CGPoint

Retrieves the content offset to use after an animated layout update or change.

func targetContentOffset(forProposedContentOffset: CGPoint, withScrollingVelocity: CGPoint) -> CGPoint

Retrieves the point at which to stop scrolling.

