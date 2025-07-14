

- UIKit
- UICollectionViewLayout
-  targetContentOffset(forProposedContentOffset:) 

Instance Method

# targetContentOffset(forProposedContentOffset:)

Retrieves the content offset to use after an animated layout update or change.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func targetContentOffset(forProposedContentOffset proposedContentOffset: CGPoint) -> CGPoint
```

## Parameters 

`proposedContentOffset`  

The proposed point (in the coordinate space of the collection view’s content view) for the upper-left corner of the visible content. This represents the point that the collection view has calculated as the most likely value to use at the end of the animation.

## Return Value

The content offset that you want to use instead. The default implementation of this method returns the value in the `proposedContentOffset` parameter.

## Discussion

During layout updates, or when transitioning between layouts, the collection view calls this method to give you the opportunity to change the proposed content offset to use at the end of the animation. You might override this method if the animations or transition might cause items to be positioned in a way that is not optimal for your design.

The collection view calls this method after calling the prepare() and collectionViewContentSize methods.

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

func layoutAttributesForInteractivelyMovingItem(at: IndexPath, withTargetPosition: CGPoint) -> UICollectionViewLayoutAttributes

Retrieves the layout attributes of an item when it is being moved interactively by the user.

func layoutAttributesForSupplementaryView(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves the layout attributes for the specified supplementary view.

func layoutAttributesForDecorationView(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves the layout attributes for the specified decoration view.

func targetContentOffset(forProposedContentOffset: CGPoint, withScrollingVelocity: CGPoint) -> CGPoint

Retrieves the point at which to stop scrolling.

