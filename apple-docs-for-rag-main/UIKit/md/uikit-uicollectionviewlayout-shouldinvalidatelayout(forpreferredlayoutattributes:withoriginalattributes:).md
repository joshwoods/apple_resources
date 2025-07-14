

- UIKit
- UICollectionViewLayout
-  shouldInvalidateLayout(forPreferredLayoutAttributes:withOriginalAttributes:) 

Instance Method

# shouldInvalidateLayout(forPreferredLayoutAttributes:withOriginalAttributes:)

Asks the layout object if changes to a self-sizing cell require a layout update.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func shouldInvalidateLayout(
    forPreferredLayoutAttributes preferredAttributes: UICollectionViewLayoutAttributes,
    withOriginalAttributes originalAttributes: UICollectionViewLayoutAttributes
) -> Bool
```

## Parameters 

`preferredAttributes`  

The layout attributes returned by the cell’s preferredLayoutAttributesFitting(_:) method.

`originalAttributes`  

The attributes that the layout object originally suggested for the cell.

## Return Value

true if the layout should be invalidated or false if it should not.

## Discussion

When a collection view includes self-sizing cells, the cells are given the opportunity to modify their own layout attributes before those attributes are applied. A self-sizing cell might do this to specify a different cell size than the one the layout object provides. When the cell provides a different set of attributes, the collection view calls this method to determine if the cell’s change requires a larger layout refresh.

If you are implementing a custom layout, you can override this method and use it to determine if your layout should be invalidated based on the specified attributes. The default implementation of this method returns false.

## See Also

### Invalidating the layout

func invalidateLayout()

Invalidates the current layout and triggers a layout update.

func invalidateLayout(with: UICollectionViewLayoutInvalidationContext)

Invalidates the current layout using the information in the provided context object.

class var invalidationContextClass: AnyClass

Returns the class to use when creating an invalidation context for the layout.

func shouldInvalidateLayout(forBoundsChange: CGRect) -> Bool

Asks the layout object if the new bounds require a layout update.

func invalidationContext(forBoundsChange: CGRect) -> UICollectionViewLayoutInvalidationContext

Retrieves a context object that defines the portions of the layout that should change when a bounds change occurs.

func invalidationContext(forPreferredLayoutAttributes: UICollectionViewLayoutAttributes, withOriginalAttributes: UICollectionViewLayoutAttributes) -> UICollectionViewLayoutInvalidationContext

Retrieves a context object that identifies the portions of the layout that should change in response to dynamic cell changes.

func invalidationContext(forInteractivelyMovingItems: [IndexPath], withTargetPosition: CGPoint, previousIndexPaths: [IndexPath], previousPosition: CGPoint) -> UICollectionViewLayoutInvalidationContext

Retrieves a context object that identifies the items that are being interactively moved in the layout.

func invalidationContextForEndingInteractiveMovementOfItems(toFinalIndexPaths: [IndexPath], previousIndexPaths: [IndexPath], movementCancelled: Bool) -> UICollectionViewLayoutInvalidationContext

Retrieves a context object that identifies the items that were moved

