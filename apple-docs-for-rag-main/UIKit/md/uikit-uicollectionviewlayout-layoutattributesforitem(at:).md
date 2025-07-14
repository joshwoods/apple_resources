

- UIKit
- UICollectionViewLayout
-  layoutAttributesForItem(at:) 

Instance Method

# layoutAttributesForItem(at:)

Retrieves layout information for an item at the specified index path with a corresponding cell.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func layoutAttributesForItem(at indexPath: IndexPath) -> UICollectionViewLayoutAttributes?
```

## Parameters 

`indexPath`  

The index path of the item.

## Return Value

A layout attributes object containing the information to apply to the item’s cell.

## Discussion

Subclasses must override this method and use it to return layout information for items in the collection view. You use this method to provide layout information only for items that have a corresponding cell. Do not use it for supplementary views or decoration views.

## See Also

### Providing layout attributes

class var layoutAttributesClass: AnyClass

The class to use when creating layout attributes objects.

func prepare()

Tells the layout object to update the current layout.

func layoutAttributesForElements(in: CGRect) -> [UICollectionViewLayoutAttributes]?

Retrieves the layout attributes for all of the cells and views in the specified rectangle.

func layoutAttributesForInteractivelyMovingItem(at: IndexPath, withTargetPosition: CGPoint) -> UICollectionViewLayoutAttributes

Retrieves the layout attributes of an item when it is being moved interactively by the user.

func layoutAttributesForSupplementaryView(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves the layout attributes for the specified supplementary view.

func layoutAttributesForDecorationView(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves the layout attributes for the specified decoration view.

func targetContentOffset(forProposedContentOffset: CGPoint) -> CGPoint

Retrieves the content offset to use after an animated layout update or change.

func targetContentOffset(forProposedContentOffset: CGPoint, withScrollingVelocity: CGPoint) -> CGPoint

Retrieves the point at which to stop scrolling.

