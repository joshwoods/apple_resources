

- UIKit
- UICollectionViewLayout
-  layoutAttributesForSupplementaryView(ofKind:at:) 

Instance Method

# layoutAttributesForSupplementaryView(ofKind:at:)

Retrieves the layout attributes for the specified supplementary view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func layoutAttributesForSupplementaryView(
    ofKind elementKind: String,
    at indexPath: IndexPath
) -> UICollectionViewLayoutAttributes?
```

## Parameters 

`elementKind`  

A string that identifies the type of the supplementary view.

`indexPath`  

The index path of the view.

## Return Value

A layout attributes object containing the information to apply to the supplementary view.

## Discussion

If your layout object defines any supplementary views, you must override this method and use it to return layout information for those views.

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

func layoutAttributesForDecorationView(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

Retrieves the layout attributes for the specified decoration view.

func targetContentOffset(forProposedContentOffset: CGPoint) -> CGPoint

Retrieves the content offset to use after an animated layout update or change.

func targetContentOffset(forProposedContentOffset: CGPoint, withScrollingVelocity: CGPoint) -> CGPoint

Retrieves the point at which to stop scrolling.

