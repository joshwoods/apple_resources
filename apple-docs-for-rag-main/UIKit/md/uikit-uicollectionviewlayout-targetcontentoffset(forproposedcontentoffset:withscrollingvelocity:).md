

- UIKit
- UICollectionViewLayout
-  targetContentOffset(forProposedContentOffset:withScrollingVelocity:) 

Instance Method

# targetContentOffset(forProposedContentOffset:withScrollingVelocity:)

Retrieves the point at which to stop scrolling.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func targetContentOffset(
    forProposedContentOffset proposedContentOffset: CGPoint,
    withScrollingVelocity velocity: CGPoint
) -> CGPoint
```

## Parameters 

`proposedContentOffset`  

The proposed point (in the collection view’s content view) at which to stop scrolling. This is the value at which scrolling would naturally stop if no adjustments were made. The point reflects the upper-left corner of the visible content.

`velocity`  

The current scrolling velocity along both the horizontal and vertical axes. This value is measured in points per second.

## Return Value

The content offset that you want to use instead. This value reflects the adjusted upper-left corner of the visible area. The default implementation of this method returns the value in the `proposedContentOffset` parameter.

## Discussion

If you want the scrolling behavior to snap to specific boundaries, you can override this method and use it to change the point at which to stop. For example, you might use this method to always stop scrolling on a boundary between items, as opposed to stopping in the middle of an item.

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

func targetContentOffset(forProposedContentOffset: CGPoint) -> CGPoint

Retrieves the content offset to use after an animated layout update or change.

